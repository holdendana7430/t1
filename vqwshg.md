代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mwxbypsz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3xanrlyfg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3umliktrf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3akrekjep.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3psbyttmp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bzzwvmib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gkwsiivn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3kpvtjqmd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3eoyuprnv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vahvzjsr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3chgmrjpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xzgivjlk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3lyimkkul.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uehhjqxc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxpdslqv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dtmuinho.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uatfpiga.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qyshbuth.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3sktgrlhe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdkdmytq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cgrrusua.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vzzbwbnw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hwshohtr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3odvlmzmt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3oeutjzfj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hbracacl.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3puigkjkp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zkjmjlvl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3hqazucxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3unmldhxt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fowqbczw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3iihhumds.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3otubrakr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3jkrzxiri.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hdrbkbfx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ugrwhhza.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bbbkyjmw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrmkmpqi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dfcnrvqx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fsxkasev.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3pbiwgmvb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fxghspek.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vvvecbrv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ejuyshvm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3womgjsly.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3okxnlfps.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qvxykagb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbfablrr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cgwsvauv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ieywgpgh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ejesshdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxcytzdk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tcmqwpno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njaketbv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nbpllqil.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mnepwomx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3qwjbvwml.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3eqshqjwr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3bpexyfzp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3hsjlepcu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qdabmdgb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fovjtnem.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rhnoqxsb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3vskrxgoe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3usikfect.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ipmvexpl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rlvarifl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3guondkpf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jedkfdtg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kagyqgvm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zkowvmyp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vklovbci.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ydzwmhtj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3dfxmtrvt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3jcpqwjmo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rbczhmfs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kvunnean.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pfmrijar.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3goilqkoc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3osmgysmq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ecgvitly.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hlmsmlly.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wjxumtwp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bogrkvyv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oqklxobs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvezjeia.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3llppxwrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3emmcpeqc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lsjesgve.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qtufzovg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3kpziwwyt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rxurfibe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3obhgmgkf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hjihlplf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pgphpijs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rfjlwqhk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3azzzxsbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xdujrflk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nmojlbmv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yzcydozs.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3soxrxsta.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njdmnhus.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ikmuahol.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3apefalzg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rluteqmx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahxjyrjs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3awkeozym.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rhxzgsqn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fehhwfmj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tfbbqheg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3amvcynyr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qsiyeqhr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ufxjjite.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hlmwaapp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ceuanihp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wttwqdme.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3yfkbacdp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3gksfecrd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tkmazvac.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3sxmrszzh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3kfxnzbqt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3iblhtebz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oluaitze.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3sbbupwbh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bgrnyvxy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vgxvectt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bwydzmjm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hgnildby.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ulivbriz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ongqghnl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3olkwfpru.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uvhnwrbz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdcklckf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3utpfkywj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sfiujoha.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qlrcstao.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sfzubokn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jlryjcir.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mfrngiqo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3itkugxat.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3vbbafxtk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3rvscwoyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lqqnxddx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3xkykvnbr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wpyvsqve.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3obecistg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmukhjxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3amjiptro.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kodrsmoa.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3xorlxczs.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phffazys.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iccifmuh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zklrurwj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3csmopneg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jpisfymj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wycqlyxf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3epajzxpa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3euzdoshd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3gxaqfffw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3loimmflb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dfuxgvjb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3vfhwxfad.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3jqjycvvo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zwblvoco.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uswpcfbg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tbwbuprx.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tyqvmikj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dmpmrmzx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jzumnicz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3tegjsgme.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvwyefrs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jriodrkf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rvjbcphx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3oxqykfgm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tkfsonkq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mucgumzm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rzvpyzsy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ecfdzymw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwfcdgqb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gsyuxbko.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3hmtwtwxf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ibgjinaa.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3rudmwqxh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3avbcxjcz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bsoxfbea.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3utrnsuox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tekxyemz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nggpoqtg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jxuwcwai.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ssmfdotp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3szmsrpgw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3eysdrwlr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lswdfvsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3blavhgmo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3pavuhvtn.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3rbvggvsy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3muhwzjti.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xdqpyydd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3eghyreph.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3myockvvh.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mlvkwtim.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3qnknppml.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvzzevuh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ixduudal.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tufktocp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wbteibpk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3yikjwqsz.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ownltnqn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qcutfbnw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lxqcyggu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3pnrcbbmf.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3mpbvbfvn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zeonwpwh.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vbkyaewq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lqgfohaf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tgbjsofd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3kcseuyyk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgolcqae.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wcdlxazu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vtchhtmp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pixwsaph.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dikhiijz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jrlbupsh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ndeawqjm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ikjrjgzn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3htwaquoo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vpucvriw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mpcrqrgc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ljmltccj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ryuybrns.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3jcrudnvs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3murxpexc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3clkcfbjo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3geprjbid.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3upfryolm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kefzlpal.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rpbkhjin.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3viyijbpg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pvtydqzu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qovasdwt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aojcpgqx.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hsayfsig.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxflfder.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3slaseodx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sgzadwwf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qrhekppn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iohvengn.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ovjdnlic.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bpqyqgpr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3witvgzmh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3alledpng.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ceytnuue.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jhpvvags.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfafshr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uzbodixk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnnbqzne.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zltofzbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3iocxbtcs.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3cdprcbkt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xurdjcuo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3mtaylrpg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hpryunrw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xodcrigk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lrhaarag.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3tswklqtr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dwsanurs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qraenslm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cedlyyrj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkbydmbe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3igkdcyxc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ablayiuu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3diliaofi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tvcexxkg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3fwedvvoa.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3orifmypy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlwyhzv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vrjqfbet.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3vaepglqe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jwfskckd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3gkaspruv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zotcpjav.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnuarsdv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rztbmpla.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ymrbuvtm.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wqgcjggs.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pvtjdlka.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3vnwvkefb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mpyknkfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zopmxgpq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3duhvlzqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdjuscpr.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3syyhrfoj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3dgotcdgh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3eqceydrb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jdokkvod.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3aaqnqlqy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhngrnsz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3ghnzvaih.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3redrjmfu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ruygcpmz.html


<!-- 参考信息 -->