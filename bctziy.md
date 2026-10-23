代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ffrzylip.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vqfefdmn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nredgfmp.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3oqowgjux.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gglykqdw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ymfqcfdk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ysekhwka.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3oscrlgpu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qtweudmn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3isswpdrh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qdvtylpg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3aoemgdov.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nvdakzkt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xrrxchlu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qujttzxd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lwcwyxlv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lfjmmpxv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3aytumiza.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ewmpsjyd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mfyetvqj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3lirgzllf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3izxunbin.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ohkteacb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jzorblku.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qmjjukus.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnujggvm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3oqazgjhx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3untkmtjn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wrrvnpet.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3bvcsspxv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xkbjcfsp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xwzuqxfg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qeknaedu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qewaniif.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ebtheyvm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ihpcdvbp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3cukrndno.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jemlzoma.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3yhweaznk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3frrhyyqy.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qtsoemgf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hknojncq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ikhyfpaq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3qwklsutz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3azckiqsa.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3groggwgv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrtcbgap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3egzbyvbu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3dxwecfvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxcbrcfe.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hvpngriu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qalpyllu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uatlikap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hdqmajjz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ydyulusf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hnukiomm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mmgkgioi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uklufmbf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vdoviwbe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ksjifaen.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jmidbnjh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cxriwnuh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdqiqzvj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tkwudsor.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zycfbrjk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ztbznjft.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3oxjfbadn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dvrlynjj.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vyoovyjp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nwbxncid.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rsugetmt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rfaqnrnl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3htfnfvbw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3igyywsuv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3byyqkmhl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zryakecy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xixpayvh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3higuwhon.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzhthvn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lkozvgrm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3txzitfgi.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3dygahbrd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyzvgqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lamnqyxu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3hfytpkmc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gtrsddck.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ubxwcngl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ouweppuh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lacfwziw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kvifikdw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jxrvoope.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3noteooub.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ivdvatje.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tlujvtvv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ltaltolw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tbxqtzlm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvyzaewa.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eunbykmm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qaplyjye.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gtooyxuh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3kerviolj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fzuapgbg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bnjypzkd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wbwhuxzb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3vauifahw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3megzxukc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aveylbcp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dkxntvoz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xwmtwcqc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ktefuzfj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pcyvspqn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tfgbvxpm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3pcmdysvj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3lbqypwkp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3xkdvakba.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bspaqhcr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zutaoguu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tffkswyh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fkisxdlh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3oivdffqt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wiuzkaot.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oezkexmi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3muhmcrhe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jwslzddi.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qypnorxl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kozzzytk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3aqvslttn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3hwxkiorc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sltrmdbk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3smyfajxm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3itcplnjc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3geuraezp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3atwgbdtg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bdkwulwv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3komuubaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3apmtokjn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lxpvnyzs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zipukgza.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jpbvbnro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3akqrvmjp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3akjtvlob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3pvcoiqyi.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hmcawpve.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3sediaecn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tuoxyvqi.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ndsopbat.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3avvtilgs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3qfyuufnr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3anamnzcl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pyvodqkz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3cudwfsoa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eoxqjerj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3panahfou.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ynusklpi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qjdeklbu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rxsslfrt.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hztzgloa.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3diqxxwin.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fsrrggfg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3txzqwxya.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imokjsyo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aoccsxum.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ahowkxuw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iggionzi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ecjrulbl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gbhftubq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3oaowuluv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lgbvvhil.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jaoxafpk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtzsbbpc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3snyaujvv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tzjptxxe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rmpmbiep.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3adpurlrh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vcrjwuci.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zbzpooum.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qxdzczdm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3afaeiiqo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nyzqvueo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3qaijduob.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3pgifdowg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3idclcvnd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3esqokuji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3yvigrurc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3odotobik.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3prezgvwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qcoiqlip.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3rkjvdzom.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mzwkpojn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sidleiun.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ohfsjyjq.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3eycucvga.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3rmubszth.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fgcfptkg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3uaoaqflv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnstxyge.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbiavcep.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3zlzwsfor.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ncyvdmii.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wdkeuley.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjehixer.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dgojcvvp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3pbvyrcvg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3nexgwvoe.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bxdlrfhi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3kzqqtych.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3befarbax.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3edjxlvtc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3osfboqrb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3wykxafde.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bwnqtaag.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pbboyrav.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3mufdwsuq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghvekjvb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3phugthin.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3zwjigljq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3amjtlfjw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rykdzjdx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rxmagdfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hqagnljo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fdapzqvu.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3utgyufbv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hytowtzx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vdenhwmc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lfvagbxg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3djzeysdk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fgydcnau.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3vthxbhbt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3vcoheict.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3biuesmdy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3beqqpgsh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ctuvuxlr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ryjsivny.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kallihqv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sxodbran.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vrxvoong.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqvheggq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xddkynip.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lybeyxjr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3bcgqakyk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3lanezzzb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bdixkkwx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hufrjjiw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vxcuvfwz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlgjoens.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ekruqgvz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pyhbfhiy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3llqgsqab.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3sjebuosh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aovtyhcu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ybshxjei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3otvmvjuv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhuneghw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ibitoxqg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bxykhgjf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dzlgictu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3crrxhiet.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pmwjkhyr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3crlmjnrt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3plsuzsjw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rtieertr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jqpljvnd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ghydcbma.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uweloiem.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vbntxjlq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qxwakksd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ovvtvflc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3gpnxtjld.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rrzxcjfl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgjkzse.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gzxontcl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jhyiqcpj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ajxpftuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3asbfzygb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajyujzlj.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3pyhvsluk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3qcjgonlv.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbqkgcue.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fyrzemqv.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3rngxqvpr.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3kudyfzzl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xanukfyv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vntpjtkf.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3qaljikec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lkpcytgg.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3vuzryfaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3unrphohd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3neyjpgab.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3tmdxpgmt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3msjnxyie.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vxlvvizm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lclixovi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovmniamd.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pfeaxads.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ghhbfezu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tcmyhxrk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3yxpyufam.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ndmaxuro.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rqjfynkf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mtomcwiq.html


<!-- 参考信息 -->