代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ecehozsf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fvzdmjps.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3llyfrefo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rtnfhdel.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3humeodhn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mulnbzld.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wrvjwkdw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3tjwrzkrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ibngtprt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3otaxmaxc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rltythsb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3qbdvpkoj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fpujfflb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xwebdjrs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mnmdzlhq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nrdurrky.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3srhsxqwk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wqltjqqu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3brfxtavo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3whgmllsy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sodxfkgy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nzedelph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3crygvixr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kwmxfuyk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ijetoqwa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmdpuxnr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zaxefsek.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wantldji.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3iihjsczm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3imxfghzl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wzdndxel.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ibtvnvps.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nnzwwjfh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oljcpodk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wzemshwy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dxxygbue.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3evqelteu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uiycayge.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3yeaoerxi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dbtwdiwo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3oddvbate.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3eyvnnuwp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3mefprscq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3hetjivnj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euqiormm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ceilmade.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3olpezvbt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3iktisbsw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qojkmijh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iutwbeec.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3izslixwn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hodpstlb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lzgdldeu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3orqetxpo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hdoscchg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gcqynthu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ohixcgnz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gtnkqaap.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iahkecsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilnvorrv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3kshgpmhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgzfemhm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hotpbhlq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zyjhghhp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hfrkgxjf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zudgtuln.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vadonhzi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3itpmwgfd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tpbjqmlv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3mdvnyvez.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mzvuxabi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ibmqashy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3blrnkpcd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kebdwdyx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3foiajkfl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fsaopueq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jciorwsz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rbxdpbpm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3sgkdawzl.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iedwxzri.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3xagrytsy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3cqvwskub.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wogoaozt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vjujsbte.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mygzmxol.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wiaggooc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3mmdafzyi.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3scrflawz.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3erfqpgnv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3efewzhys.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3oglvaygm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fiaoanth.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mfcjtnlv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mvxtgwzr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3thwetlvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zgypydfg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zamtttvd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3igciprsn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uqjypzwp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xpcefeuw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yctxmjww.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3piothmqa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3nxgwaroa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3brkblxag.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wktxcoem.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jgfhnewk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tsyllqge.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xlpgnimi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tjupvuqq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jgtyvqpo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mmvugbsp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bzpskifm.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3oukjtmuc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3clbrthtk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vxmkypvj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3kwihbjgg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3vgdpxbgq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xtvbfbov.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qjfypigp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3demoxdte.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nblsdpli.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ucwlmjyg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ryxvlexv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pdvtcnis.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uesoqqkm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rmetaggb.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xhzaxgzq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tkfyyzzr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vykefyhk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqfyqoxg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3hnmmsdkj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3kpdfndgb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ddfzfwzp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yrjtokrf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3hjkrhnqg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cvonerqc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buburmud.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3uevgdfch.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3gvdkvqgu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tyxuzwlj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlbvlnfm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3txmqszzo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3awcmdfzr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xwmpgxql.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3oqvsmbrz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hkndtpla.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jxtkvbow.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kzofhvql.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aejdbooo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hxrphani.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3vjzncvnx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3lktabywl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dyijgxkd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dhqxhoun.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pudvhxzq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pnkmxxrv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3jxjplsfl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cfviffju.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oanlqppf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jfqgkmez.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hrgngfjc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ylifmeqk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gfoupguy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qazobrxp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xknaqgll.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xogcontl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ecivtafv.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jayeuxzb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3devhuicd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iabidcan.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3kliqkwsj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lmpjnviq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pxihbnge.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3aikinkia.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iqajvlzp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3lqnhbdph.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3agdrjvjf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3qjirrmeo.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcjcwykf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3nozvrdxl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mkapshgw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aotzxyry.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wakfeqgh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pspejwyw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcjfxjkj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ektecgvw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jgyjjkzr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjdramrt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ekycpxfn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3mcukhvnv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3faxncouq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ucnmgiyy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3coqhhwwg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3pnuprgvn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yzmjrgki.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3tdsrvwsi.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsnqyxda.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jyaqronk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bxmztlvj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aiwhnnfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jcyktjbn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ywrpiryn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pvmfkkbs.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3kowaghtv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pssrdbty.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kojuvrhe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3txyuexhe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rjnvjhjq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3jthdhgcq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3tqrbdypq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qxmcjnaj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3qcopsseg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ubieqctr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sgqawnjc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3gbpyffuc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yejfpcas.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3dfaftqjm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3djasqjfl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uhvomtzz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3spkyiqcf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oxofrrsu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wywhtkbp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nhujvydp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sjthzyzm.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zeogxpjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hxmbejff.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3bdwvuxah.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3twekxjvc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vqzltjtu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3jleqzctf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3rjgihfby.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ebsuhudl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iqpybxzq.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nefgrqrb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kcechplv.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlrlbjaa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rjukysqq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qduxrqjp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3onymrgqy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hizkfyka.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3gbynbkdw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ybsulpfq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3lmuesgtu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tpohkpko.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ifqubjdq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgtxyxwe.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owcgtvjj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qzokuxbz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgwebtyg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oanfwphp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jrqdnbkd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3jspzhcyc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aykhksia.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rafitqip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juabrrjk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3woresfjq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rtbmplga.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3casluupc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tdbltinr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oxkgdcmz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3qzbgxzcy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vennyunk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3oevnscku.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vnnxevwg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdeymnu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pxznyiqc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3iskuawfj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ocbacnoq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3xznurcwh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hsaekfie.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sohefawx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vsoqtjbv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hwyrhqpg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ksndduqf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3xsklxdqy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3kllteqog.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fxbbswxs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3isykoujt.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kohpgtax.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3dooazlib.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3cezcqrrn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjblxdp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xwmcxyda.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3tikjvhya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3oyhumden.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3asmljfhi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjwjhyhk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wnwqvvuh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ahambazs.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xyjgovvi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rgkjsxpp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3avdzwpbt.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rjajtxwe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sprainzt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nptzegco.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3typmhvuj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aygbzsra.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pvkzqlvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwxcbdgm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3qvteenwa.html


<!-- 参考信息 -->