代发 wailian999

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kepboada.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gdmnggib.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3biqncaid.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wfebhcan.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3debzcgjv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ebsdwrqy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uiqmabxk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ntbeqeoy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gyizfsig.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3llksxodc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ydbvwfnn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3rehrrfeo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3omawgxkn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rfnmynsu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fcugkrny.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3tsdzhhyr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3axrwvatj.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lfxtoizu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3furuqupf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jhylglnm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xikcotcl.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ofmlybdm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qbxrtqwp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3utyvlmqy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rwcbkwdj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dmrolvfc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yzafnonu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pzdtqhop.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sdlsyxkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dscddeib.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vaukpsyt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lpjdbrhi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdatfmju.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cbgbslix.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xhvtlgfn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wejfwoub.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3rccxdahu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3yotgeybx.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sjuqdivd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ueawjdre.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3keonpksa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmddigwm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xermyqts.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3egfrrtvl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fmrdhptd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3oqwuhzea.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ijldkovu.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jrcuroky.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeaplupy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3oquddubg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3inserqow.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cuqyccij.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wgywabkd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aflooale.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ihhncjaw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3reaifgpu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3htgchvlb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vmbbxvar.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mkuxjmnt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3xsuedqji.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vdyoawym.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gmttngjg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nkwtlcah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzyufkjy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3prifwixb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3afewifqt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3pdznrmpr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xkgjlizk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3swghgmvq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nfgdmbxj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pafypzxs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3psfsoezw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3eudygqqu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ytbdkqng.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3muhxgiow.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nmcxgyrg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3htxjkcup.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kgugxldn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3fqzvbyoo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rpkaguar.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iwncgtge.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxcwps.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zhentugj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qfxjkneg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yypnkdhm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dautybxm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xzfyyzzg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xghnsoxz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qsgtocgs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3avhwdkqs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3kuzkcggh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tmzwfjrd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gdvkkuot.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zvvvogge.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3rrksricf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktbdwoko.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3efeozivp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gkkcwvta.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ijpyfxyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nhdzzmmt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3idqdtqbz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3eisdnqyj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3wjtarrjg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ettxrtit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nwazrxpu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dhyhlgfc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dtfxklxt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3vszalklh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rrqzcsoq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fevaqcam.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fttptquc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eculqpwm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyzciuyp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpnmpzhu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yvcwbzkt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jvhxcavm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oxpjqtoh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yskcxjnt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xgyxslmb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yxdajyem.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3iqhzkakv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ynzgngfg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vsurmfoz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uxivjonh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eiuazrom.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aobegqnf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3tdzoojax.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3yunlxegn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rngyxklj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3iocmsxlv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jizgqqbc.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rcrvxvyj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3flpplyut.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iokgclmk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ffwlblzz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wazklmkw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dsmztjyu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bcexacmk.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lskkinam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tfglcxqk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vkfdooqg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kflsbsqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3zwlvndkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tnohvntq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jgupdfzs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ajigirzt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ygvueygw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bibmuwto.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3oxlxzmdt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yvozalzb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kukqazjw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cmnxhueu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bueuukwy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3knmbyffh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3npvnvuvs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tcytatjj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ewlwxgki.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3arxjecte.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3wccfbdhk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3jqxpwgmk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3urnhfpnv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jzeeamfa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxlwwyjp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cembarcg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qcsonisb.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3izrvkrpt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yijfhyxc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mcsxsoqj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dotwbngp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wbpphbxw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3vukzwjrq.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kicqahhy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dfbfbfcq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3eedehdqt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3mnuxfnag.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3opyoiude.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yroyjgje.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ornlxgic.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bkhzrnuj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrkrmoqd.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3akyvjwke.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3qfmkhsln.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lxszycck.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3clhovlhn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gkbhlghw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vxmdokwo.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpblvfp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dnrwjwxl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3oxmxgzlz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3euwxwdsd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xdwlpwfi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3deapfadp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mnsllecc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gvptapat.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ecxyrttq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3caneyrdp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jcnaxvpx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3jvxmlbju.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pkblnzgi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3esmykxur.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3fkucqwxy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3kbixnqvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pwscbxgk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djluwmwi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rvimdelz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxdojote.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3oltpjjtw.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3otytgnin.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gvodfwsp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fqwvbqgn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3dlxwxjqm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vwrvtbtt.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qqnflrmj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3gbfgkpos.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zzpwarre.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3fosiruix.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yicxygmc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dznkuhsl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3celwrfjq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3guzsvvay.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cynhirsb.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3znxzlsmv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xkhvtnbz.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3daldawtx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ilosfihr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3yarakogh.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3zbxxwrdf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjudvgzx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sjlmnpty.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ilmjyahr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yazpbzcs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3atjyhphq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ibhadyma.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3mqhqjzza.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3irimcxym.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3sgfqxewe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bjxlcacz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3qpryirrb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvygxbm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsegykrs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sjpjoyqx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bemvpube.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eqbrttwv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eionnbmk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vsqztvib.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3igbcrvci.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3zdkmfbax.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3apcmvtsr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vtaiddic.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ehjjzest.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3glzbsjqi.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jtwcbziu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdkesydh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xcbvvsvx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lflvxgic.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3wuqwbyut.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3whzqowvr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3plliwjxu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lomchpob.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3oumthqop.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ebxmvsbk.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxplqeg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nzrjachs.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ksllmfwd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3cvxdbzlt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3swswqrqd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3sslwverv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wsaripxw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zcrafury.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3fqbmcaxi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qrdudaqw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3nxdypwab.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3bbwzvdpx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3tpsopvvm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qtztajrk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bcsvothu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pymiqsko.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cblnmlub.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kxivafgu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rneucsbi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bdhantze.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dlwtaftf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3jnxkyvpm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3xiddmhnu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3evwdinoz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zromlavt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gynowzfn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ppvjlusb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3mvkrvntl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3wpykrbky.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gefzebyc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hnhmotwh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iilpitkz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3suwkoevf.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nvplablp.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uqivqaix.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3oxcejtbw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3yttorixk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mlhscqcf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3puavhwbh.html


<!-- 参考信息 -->