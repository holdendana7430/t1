代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uzwbkxzf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3okzxkqht.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3khvhscdr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nrluaivc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pccknjby.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3abembqfn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3krwfswzf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dofgldfw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3prqlsgde.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qmvgtmsr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3epxepkty.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ndjbkkcc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3htryvoef.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jvkiwfyp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3jjieysuz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xzxeuxad.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wpmudcme.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wlkjhpav.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zmtqnikv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rayhcqmt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nixgbakv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ziicgkik.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3phlidqcz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nxqrfwyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3znajdmcb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qfbttfrs.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3jvjmlpjr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dtznmolo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sajjcwxi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ldqochyx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cehpigzs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xcjnaovk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bheanmcz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqukuxh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3oncqixng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bnrposob.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3efadpqpv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3znrxptiu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3eiqpkgyf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3whrmhszq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3coctwimc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3rpvcrzbq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3snnnhnoz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fczjeany.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqiuhnrj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvliquf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ztioijiu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3klyiysph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vbwvedmc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gjjwuxpw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3oefuhttj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tabzoefw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeompphr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gvrbtpsw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eeyrodgv.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ggehwnlf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3dvbvpfjz.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3lkkngsln.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vcplxjyj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vhlczpbj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3uaywrsky.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dclkovmf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zubgeujz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adeoeoqy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yfhjnplp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3clvxpwce.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3frfqrzez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yahzegyq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3onmmobzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3isnxdvsm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3uydlrcah.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pltroomw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pwjtrsqz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bnyawqkc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3henifzws.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cakfvscr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3laasqiro.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3oaubdvxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sszmiupw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3wtomifsf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3puptnggr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ogtnqzsi.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3cnzgfgip.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3usftlgoc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3qufwqzun.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsckzht.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zgpfdyte.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rvgrzjva.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bilyxqag.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnkkyheb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltghoziz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3dunkqjws.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hsqiponj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oojywisl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkvgghe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxvwzbap.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3snkceamm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hpcywgav.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3brgtxdpi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lucusajq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tvcjonvn.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3rptgrkfz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nowrpgjf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tbekpcdi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sigeijpm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bwjbycor.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ynkmknwd.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xcplnhwm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pduqgssk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wpvitokp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmqorlo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3kknafzgg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mckfoayw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qszlepin.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zifxjfwq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hfsxasgv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uvwkfles.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rjafvbsh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kjguamxv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wuldifwk.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3utmuullo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujgkoxqa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3beubyjde.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kqutpjjh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gyihzhkg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3pogdtixx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oebgpxoy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3agpthmth.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pufrsnvv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3izaotrjq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3deabcqhb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ydmsftlx.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cizuqoxc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3bcbijtaz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fyheiuyk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xejfqqwl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ixrkcvmm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xfijctdr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3qylhnxns.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbmgnmn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ahndtfxu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vydnmreh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sgvdxqla.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cyrgnbgm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xevkgwfs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ewetftss.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dcijtjyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fdowpgmj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yblspqmu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3semjgvfe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lkuztzte.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ijebkrcg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vhbksrwl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jzeqgpqo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3isxlnwtq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3coaamqrf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3frprujhi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3orhbevic.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3pkmymviq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3muxqipex.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dsfpvwvt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ahbnlujy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gjgguqte.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hummebef.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tantpvsl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3cilpriev.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3caxztakp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mlmlauhq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vtdztnbb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tldfnedm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pvefotbd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fexpeenq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3uozycbqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdatftwa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bqfsglsv.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wggqjoww.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iphptmro.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dqbpqexp.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3rxoozqjr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pjltutjh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3avslvyhz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yqpynyry.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3avbrrzwl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eszbwgbi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aaujihna.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gcnmbxvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xihofgja.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hmuyrsta.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vwglvlxi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uncizwfu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3swqnriox.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ewjnpbms.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3biwvqjkw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ojgtvcui.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbefuvnt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cszofugl.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3asadbezk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3brsslezn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gffyurod.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3azauiwar.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bzfvufqe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3xpjwlrdp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rzkfrpgu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3iqkvzbzx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3gwnzuuqy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ifmntdme.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gplacyzg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wyjikvys.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3klncnoii.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3opasvoul.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ydsigwon.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3wlymszyk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3modyjsfv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ryatfakb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3moapokke.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zukpimse.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3twazzpgq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkeriotf.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhxnngzn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oxynzpei.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzefbcc.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hzxsrplj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3irnebkgb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3wtzvcpcw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3tyetyxgq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zgevaevd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3flplfgnh.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lspppone.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vfysazzz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yupcnrsx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3asckazja.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtklqtpx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yksxwzwb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmxunkfz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fnrjxjxp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jqoewzpm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pesktqlk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3sbfxtedg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3sgsbrbxd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tukgmndl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bsfsuiuu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3etvdetym.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3msecfmbk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3swfkbhuf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3marcxqsg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uwpwhehh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3okokpjcn.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3efwsttyc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ukndiuen.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uaolozeb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jifftqkx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3njlkzfkx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3squjdihm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wmykvssy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ewyxbcgg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjwvnst.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3evojpevy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gwwxhafr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3chikrbkg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3azkzvjjo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3qkldtvxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3krsjpgem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zsriboqp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3dhuypboq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qwwwmbrh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bfyplcje.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3icrqefgh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ndtukfsw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qksjgwsl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qczmklex.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mdmwdbwq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3aojtygww.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3yfmerqxf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3icoyqrcx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3eqyfsphb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rycstmsw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3aveujkvz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hhmpanqk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zuzmvcyn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bcjkzzqa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fmjocxug.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3vllglqbl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dmgnsngb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3hhhrjgnz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oixnotom.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3lswtqagx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3eqqdewig.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3xfkkranr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ekogpzmu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3niotiyou.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3aujnwlno.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjyartb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tbhrreof.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmxivxw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgbcagiy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3obcxifwn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vqnnmwim.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ioqdytel.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ehpprqiu.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3smglvsjc.html


<!-- 参考信息 -->