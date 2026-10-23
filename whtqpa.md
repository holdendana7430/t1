代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bzvkratg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3btwkjnua.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3hkrjxpnv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fwljdobi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tralvrsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3aibcofdi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3flflbdge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tzqzrcwb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rukebucq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cbixeagc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xkzxxofi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3hjszskwo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mxcvgkwd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gsnboeoz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3mtthfshu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ofacnbzy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3svfbfstg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rshfxkqa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wecqznks.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nnlzezqt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kogcbuud.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3nxiglmtx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3tkvmusmk.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3qnijukdf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ijdnyysm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tzgofcny.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oqfcqukb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tvhczcjt.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3katruzcx.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hzoryeuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dwiixyrx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nsczgwvw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lrgabfwg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pepmpwsy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nibqwnnb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpzykasl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3douxxysh.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ozeiiavc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dobyapsl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yowveypv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nvmmdjrg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nucucoob.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rcifrmrl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rdipzhwm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3onrzwtnc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3akgedmfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3hqnmgphr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jecvxivu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nalldvwy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwjnlzct.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wteexsgm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3sferieru.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vxipmajm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eszwajbq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wyluexgi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zpzsyety.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3eqmlutor.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3irmfxcmo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3anbktljf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nocuvjdy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mpoptgyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3pmizvxwp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vhzzanye.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lidqjxra.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bgagmrhl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3hnptcnow.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsfwumhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xufosgov.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qpbzagnn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3harjsqaa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hcezyfmq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nrpnxnnn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eccryutq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cdezcwsl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ijpitklr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hpempefw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hehvcpkc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kxwqkfic.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3iqsbalfy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bivwspqm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3feaumtap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hwxneycn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fnmlvoaz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eaalkizz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3eqrkyivm.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3sthbezxv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rovbkiyh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dreavutg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3zafmliut.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjiajhft.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vkhmbktv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dbjwagok.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nbiyrdtw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rdqymigy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpqzlcp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3svrallcb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lsukuppp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3noolbjsa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcvlotlb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3olbkruut.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bvdqcnbs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dsbfdkwd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qiokdtcp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ysukwdzl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdmsivvx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3cupigdsx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qgvbujbx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uvimlarv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3quvtcxly.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3khxrdcbs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3mqmtmzvp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3mtzeowwq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wnhxbnob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3coiwqgke.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lznpdtzw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3npzerzwd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pkipkpok.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kikgwbxp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qzzrrlrw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dpsvyibb.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wqyxskoh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vugymqeu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3iwbhayyv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rkuycuzs.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zbghvjgb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3imrhzkuj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3cdhtyfkb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hgyuzpww.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pguinsjg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wpdksqpo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qapqvlbm.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3waimiilq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pkvxlfhf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gzbghsiv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ukcxakuz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bqigcppf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3obqozxcl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vacfipbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3trwfictp.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3zvxxpunf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kkitvanh.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbinxbmy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wxxfepbo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qqymgwgo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wrmtndpi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3xhjwtqba.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3axzxttxv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hhbvcyer.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3fyobkrkd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rpbtclcv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ynawisxq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lrqjgqee.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3azonmdhd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3npmjuhjr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kgmggate.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mmoebswm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ayznzish.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eharomii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hzgdgsxs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tiqnrjwa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zevpfvbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dtsgdmqu.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rbzpgkgm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ehvlanxg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3iwnpthob.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zxgsnckp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3umqpsfjj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rvikluwz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mgprclns.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3wpqqojsw.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3abgytpco.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bcrymbcr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lneprqun.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3djmdxibo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dukxalod.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhkytkga.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rukjqejn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3obcmrisr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3cogcbgsl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mjbcjfaa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ojabolya.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwrzeggi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3uhpyjzmw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lgobyulp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dqjodtri.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3uqwtzxse.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jngzrgit.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3dmnufvtv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3oelqxepl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3umxwigbe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lbkdkjzy.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qdpayhpw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jeoimomu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fqvolgxw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgjvbrxg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3deuuycpy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3rrcvbjod.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vhvlowxo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqbhglea.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nlijpfyq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3rxiayyxs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iqngmatg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3kvgdbjic.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hxsrmipo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pcsyjbls.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xlfrnhek.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrrflqrz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pdtzvuzu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mtohrvmb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3abszmlxs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tstywgsd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3soklgzgq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gsliaebz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yffednvn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3flzedlbg.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3doexoyio.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jecbwdxd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3abgjjayp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rufyyfdo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rioofuzi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmdqxfo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ptzigrfv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hmkeysxh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jajezubp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3mfhteegn.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3uzypvbfd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wcbseffn.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mcupzusb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bvkprqli.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ppncfpmk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3doeoblhm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3npidkxrp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lsnuxzus.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rndklqqt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mmxbdjot.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yvepriwu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3enaqezfm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3guookpiv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mjnqdfic.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3tdcoalwt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ejniuadw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ejrlnxwb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ikdusngo.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmhuiedp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ttoilffc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gtxdmepu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jarhabot.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3onaciumt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ctthemna.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cxgdgjxp.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3igunyayj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3irfgkyrf.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3lhyxfccc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jrrbqdqi.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnzhgjp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ysovtpot.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3muxjqknw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mvzajjwz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3onnlwbuv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3grmhxsoc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3vtunejsw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xalwbedr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwhvjgfc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3azbrdpjn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qvztjfsy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ufqvcjyi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3gpueasjr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fwbcddkw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3diduuowq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yygwqxzr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pvklefji.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zgyzmhpv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tumetkie.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3sgntvsru.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ixfhlvvc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3azruxakg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrdlfxlm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ajleinwj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ajmnyptq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3towijyxg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cozovxrb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wsmkmaex.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gbmvbkli.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3evaxofmq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3frirnewx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bnqjmmlr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3goscknjg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pdmxizqv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vxysjmfl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gcgbtoms.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3okgzfmik.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mmycqivx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ksexcmme.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckumnkva.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3knrzkvsf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mzogchuc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zopxysuk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mgepyskj.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3olepckqt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ynxzzrko.html


<!-- 参考信息 -->