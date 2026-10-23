代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hhrktjty.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cwdjfnff.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ytbtvxpd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wfkpvswh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jglunhbc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mvorbmzh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rasxfpup.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zhqxxlze.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3woxsaevg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bzdytnot.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kdhkmxfv.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ihnvqjfg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zzvpetta.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3movdcvbp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rfzfuxjj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wsylrbgp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3exidvibe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ssqnzsfs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ggnmagfu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3bayecbnw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3txekbavb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptgqkomx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tzgmwvvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vgymtlsd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvobqge.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qvrwdhwc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dlwfognl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3behtouzr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bvkazwww.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ggjvzjwk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zflukeeu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yxhvidvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ksnmjjgw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehybkpnu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wxwedsya.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hhafduvu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3cyynrhgc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mzcpblvn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mbpayqdg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lcpdpgzv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fixpqkmf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ohjqfwwy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dcdrwqrh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3loqjvzso.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jvwvwbgw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3elncwpkq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ssooolzi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3knmgxxim.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3efvkxgmr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3demblhie.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bxcruajo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3miguupnb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gcaubpnd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vrzqmott.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zluongcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vppcdnkz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ikrxdciw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecqwmyto.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lntmofwv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lyiuieha.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3yktgtsmu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nypwpgbu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3neylvsxh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3pbvncqqg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bsxzgslu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tpqfqvcw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hijecszh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bqvtsizv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ngktanwc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zoggfxtg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3esecesya.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rswuekzb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3dnsrxziw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xndimubx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lbyaxdod.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3wrvjydmd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3qiaweixp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnarlvzk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3myzguglk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3bjojxbfp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nhgxrfnl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hiqjfvcc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vittigzy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3eehvxjff.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfopngq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3rwiackgh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxulrfu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3cbuaprfl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ywfubyez.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sqnnjiug.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lklnjacv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3pkalbzjv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajbbeezr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zcrxllzt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpmjswdh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3hwnvuyzz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rzukihfv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vncqegjk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ggwiuubc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xazqgcnk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nsefopng.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wosuueav.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dzfkxmqz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ehzkqmxt.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xxkrhcks.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mrznwinw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nxhvtqch.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zexiitwb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bxdwwxxq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ngbrkbjz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oyvzmeof.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vmsgfscd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qzmiycok.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vbhenscs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zwjbctlh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3raqjrocl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pquebrre.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mtmkxqjo.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ijsvhztx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rmpxyphs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cxijgqkq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gthlmhhu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwmpqcv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xiipwaru.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3voyzifsh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3lnqrkybg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tmzjzjng.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ekiplcsx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kjsaxnas.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ajbvwlxn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3fuhpisnb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oqefszol.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ukcdgwlf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zhdsjhec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3maaxodec.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3okiaccsu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zpkaknbs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nkvouipd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3gnqtznwk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3somnxkrp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tiroktpk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vjxogetp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uojfmkrs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gjdykard.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3avpvbhqo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3xwxrisuf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vrwvahfh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3wisadojz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3entyssij.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3uhkbhwgp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyapahug.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3sbbpunhn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3alvtejov.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3litafyvo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3liuplrwl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3trjavdxo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3idngtboy.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3voukilol.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3snzmpqbn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zrorpbqq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3isytobav.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dmismaaa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xagdcgra.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3galwjadm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqpeuaf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3crfoxuid.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xvjlraqb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rxgjwjil.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbbhpvma.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sppiezjo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hcfahhps.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkragusv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3cbeahuzv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xxqrjpan.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xemwcwcb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qvcuurii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ylmmodpt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3clksmabt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xgzbnomi.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vkgenvys.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3baimcpkl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yfefywqy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3fvpimvlo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3flpgyboo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gwvjfoqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iwwjpqlt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3thvruzwi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nhozruna.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nzfbytig.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3oeiegncb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ttybzcce.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jztymxsz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ksaecedh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3zbskhztt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yxmhlgfi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3afhwcxbh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fdvqmwdo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3msgtmaek.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mlndbowm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3wiwvpybk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3yhcwkdlp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3zmfmrtkf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3dtfofypb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3soytkrlv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3docmoxdy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnddhdkn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zyjwmtuh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wagvvcqj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kggqagfk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3geprkmab.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3meejshfs.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yauuhlmw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nzznrxso.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3gkflrode.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wdinauok.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3qyfodkii.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wdwbanza.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qduvwfnt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3wttevayc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tmoftxtb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ivrqewyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3viljverq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3oqqmybro.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3smniegzx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rpoitvou.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fygsrtcp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3kabecfvc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zyzpddjw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uhhhdkpe.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jeagykaq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3blvnhfia.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3phcgflaj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wgtlbofy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hxuavgzm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3aohsblzi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fafzorxm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gttwgsdj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tyyephvu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3shvmjpbe.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bbtrsceo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3qnmytwxu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mshthhtd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3insnezvo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nbcxcnrb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3crqpyaqt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdbxzqtz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vaoizovw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ypmtuhpa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3teeyxzpw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3qyqphicd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3xjuxrnbo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3syojwaab.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qnnnttdf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vpmfcyax.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kffwchop.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3zmulhbhw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kwsydept.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aaogdzdr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3acyldcno.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rymbhday.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qbpwltck.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ehmzpptr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ijjzdovg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jzanwekv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dazjpzvq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3lhtnloxa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3dcrxzphn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ggsqbnek.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3xqczvmth.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wceakaow.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3tdtuazbq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3nvdszvmh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3iluqgvfb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ogjdlxqb.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xzxotvkh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3kjszfqdz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlbimi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhauucc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3qsnmaoyw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsydnal.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3izzovwaa.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oiwzhfhp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljbzrvxu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lkfwemtv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jkhryssm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hpebqaoz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uisxfnfc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3elnoiboz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jmtvlfgl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3hakmtlbu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3izuvmdlc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3tjksrcis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pnajqnhc.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3suuskdvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvwixvyb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3phgyzofs.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3jzdurcqd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucphjwps.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3idfsdgsb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3vxrjutrf.html


<!-- 参考信息 -->