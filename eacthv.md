代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3qrisjiqz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ongjlatq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ekweokas.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ipebdanf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3umypjinc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwuebcnf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3yfsfvnst.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykzlheez.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lljrfuue.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uoyrvpzd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hsrlqzoo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dfeazacj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3clfbaryr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ofjmpqbi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lgtennri.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mlqkuabu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whxqnzis.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvkyotuq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3geylidzs.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rsaeipgj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ffkutlbk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zxzdkoni.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qybqxjey.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jxjktebm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aeujwruc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cadmrvhf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ehupvpmq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mbmxrxob.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3sufmzgfj.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yoaszjsd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jpuyhjjw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xntvpjbz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pcthcsgh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lxbbkxad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ewuzkyva.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3heitrxpi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3timoslkf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3uutyxygz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuxueofc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wckpfply.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3xhfdwghk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxpwizmm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gwuemdia.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lwaejdjm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hcbaxkwe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qzvqpcgb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tlkarrkg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ebyueike.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lsuwejdw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wgovzyms.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3dzwbffvf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3stfkhkyj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3avqntubr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ojrzhqif.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3czumfgqc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vdffuxah.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xwpzmzhx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ssihlrmb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mabhuwzk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xigstadj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mbrmevgu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mrepdsvw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hrubhpgg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3qwpuapim.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wxeyettd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3bfcasjhe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tjrmjfxc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zyjlvvee.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zgyvvsuj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3wgboriql.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jizgjswg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3czbwyzqo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3qjonaius.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ovfedxtw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zpjzynxd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3mbhamqjw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hlcvcdyh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3iyxqbpdo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3khvbhdys.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bthwqgoy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bemdglqw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ppcpygio.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hqntliwd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ozhqztcl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bjoprszt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3epasycns.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bkjtifix.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3sphuajia.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tljylemz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ueitvung.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zljscftj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ziipexfv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zyxxilms.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lqloypjb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3wohhssjz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3bdrrmprh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3axypbgkd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3cofjlcso.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xckyzdiq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vacarbxg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tajptvvm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wynklypx.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3efqbykdx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lbahbdui.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mgothkrc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vcwojiev.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lxluwdyg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3umdbjlqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ehrovwaw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3vqikurml.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kvywscel.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3qsziupwq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3psorgapo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ivaghlry.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wrhjbjpy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lemmlhqh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jjefwcwf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3yufpviox.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qubgucwb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3jasceuig.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3lzbhhgwc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3koaricfk.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xwtgqvsy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3yswpoxed.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pnxejgch.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmkjugtc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mafworwi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dskyaswa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tbkglusl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lfqjrcfs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ncpkiwtw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3tntoolvm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sjlhcpvh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tllgpgdz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3npjqeiin.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ssocxshk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dcziruuy.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3upvejoam.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zxwrgjxd.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gnrxqlkz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3udrpuonm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3nkeurknd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kabsvrab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mttitdtw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3eodbphjx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3olgrerkc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zztapwve.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzikytu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpwdfjae.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3czvdvptt.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bzhncubj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yxmutatt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3fyylyepg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nddpjhin.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3djqrtwke.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fbujvdqs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3kloirvtp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3mpbnvgso.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gelnynaq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yajzwvgx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vqmylhju.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xctbselq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pctfsprw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqubzwss.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yftsrehp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3icsxdsql.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3daamdxbr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3odjhfgvk.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wefxjadt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gfkbnovb.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rapxqfxr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ntjxydau.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zjbckoqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3umfdpmxa.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3qfegagmn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3rmpipoci.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxrmowmi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3giubvcbm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtldspds.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lmlgqlgk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btfzmhoz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3svvlwgyp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3egkbvget.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lykwqvqq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zonmayoj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3tusqxwjj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sbxrxopt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3klcmxddi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkrodnyo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkmqvhk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3taujljxb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3suavudrx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxlkwrei.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3xwghmlui.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ajyrdhmy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ekuhteeu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cgslmzva.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3whptngmn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3usuwlayr.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3dhmcqmmw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3xkvhzqyw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qqvsuixl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3walixfvs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkgjcbuv.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3eoxlinov.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3lmulgphz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yliasxqb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bkgxemkj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3umgxlozh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3imhextza.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3erkunhel.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3swqlsygt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3xftnxbkt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3sqttxqek.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckitjoqd.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ypihndar.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3mjjsovwp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3evsrlwvt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3aguctgjf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dslfcmfx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3klymutvx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3hdvalipl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3fvhfkiuo.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3whthokpu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cisydggm.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3afsqihci.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbqxouf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3onnvtjwo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fmecjcag.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bhgcbtko.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtjmzej.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dgozzfmr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsitxodj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3mdrgjcmb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jogslrvi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3rjbxmzfd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nmbptlmf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3lemxpgum.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3bntexrjt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3yqjlmhqp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3bnunzekl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3arfbcudb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3pqxyjchr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yazwybjk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fwtadumo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3abhvgovr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ltjekvzf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ykmcwetn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3cmcwcjal.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ehjkejpx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3usvhdohf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wrqoiikw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zuscqkda.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3sxgcgazu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3wgwehoiq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jflizowd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3hjynlfsi.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vcksyfnl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3reupqgrd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3havbctje.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zbvdkovi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oiggpxqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3cqykqwoi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3jqavzexv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3cuoymwhx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3cpdufypd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3upgjwqew.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ndxjpyru.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xstbicqy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jfjdrszn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ndxfwyes.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zpjrtehi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zfflxwuz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3dqybnbsw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qmaeblgt.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fplbbcgo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kqdouvoi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hpddxhpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtbuckwl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3pygeclim.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3hahugvpa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dpdxhxou.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qdgsyqgn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bexauhza.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3opoxllyp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qttqifku.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3uwulbeot.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lezsenlg.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3glmgozlr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3camlklgm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfqqcitb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3mqlwywol.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3lkpouhiy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vukogpnz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lqjkgdrg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3tcdcjyrh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ugomxbdd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3evoxsodr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yckmqirg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3trabiwsx.html


<!-- 参考信息 -->