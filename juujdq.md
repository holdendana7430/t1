代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fhgizwjp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ttanlkrl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vwjafcko.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3edlzcfav.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3rbdeiuwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kvxeomtc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kjyfwjdf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpsenvmk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lompsnax.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3biltlftt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uhsdrbsd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3obqzdkwf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xdenlnam.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3iskvlxrx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lrokesew.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cddbweoh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtuwwxdp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hfwfeubw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dqpodqfy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lhfjnczo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ebgpzdul.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3hltucrbu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wpsuqnte.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xvmusflw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qgcdowhe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kesvyynj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ffczfbrh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cdoarjye.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ndjcsrhy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3aploddvh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3jtuoprtq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mbrfpmer.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wmnfcrvf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tnnuwpsl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3weeroqhp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cfpesiaj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uowfitbv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jutxggnz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vfiagyzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkkdjuot.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bguofdwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfgtfjka.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nlsikuhh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3mxrtsqqw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ieztogiz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3kehrreea.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yowvkfix.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3mdwrqrtv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vwpagfzg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3irwiawkw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rcaygjja.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kbrciikd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eiyevybl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ajnuvqyl.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwostoza.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxfxnrxm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uatpsbxb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vplacxgy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvqmkfu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mjrqqgmw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qzewsach.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mnglsnet.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lnpfxgpt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wukwjsbp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ugmqdboh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oumclgkj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3wayarswz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vnyrveih.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3umgxuszl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3tiayfvzs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lilylxbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fmuyqiss.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ynsklghi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hdxhgrol.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kfcfgvue.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tosxxcjz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lrgzqsuf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ovwufwqk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3avvvzloq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpsmxt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xjsvsvxp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3loqliepj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yhqsgwdt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qnbhuzru.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jpquomlv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jbhldlgb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gwrytvwv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hdpyozuj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3yoeybiua.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bnxjtlip.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3etdxgifb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3qtmiofbt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ummiflso.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lkoljasm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3iehqaryo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gbhozzad.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ssilcpnw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qnwmlpee.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3oxwyrsvj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3spuzbpkk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jeifslyj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qcqozdnj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3iqcgjldw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eghdeidd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjkqhwdn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yemqpnkx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3utovpsun.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3uwmblzeu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yhbtmmlk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ymxdkrix.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wbytcann.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3fuchcgjf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3frsozdxc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zswojjpj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3uwqvfoym.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jcgzkzgv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3btndtoxi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ipufgnnq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3apforegz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rbudyzxf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgljewrj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uwikghtr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pzhhiaxy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3iabffrjj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vspewuua.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehtympye.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ziawisqq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vdrjgjgz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tsckrogj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rctcdshs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjucnlj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3miwdrdez.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tvsihiam.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3edmtnxjq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3puwvowhu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ymmgzocm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tzlofexd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mhmbrqkb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3qaaznhpv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uhxkmaut.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wlflnbwv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ykqnqusj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gvgnsjie.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgtbhzr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pctfufae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3togzrqxn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kopsxwrw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qolztqgo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ahshklxm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qcwaoloq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tuvimcoz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pvbqgjmt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jymrhdct.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rsbkamct.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3waczvppc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsxaiuow.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3givrdgal.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ngrrjtdb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fbsnqvoq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vztpgczu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wpyrjwdn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3carepjqx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vxwpmdgu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gmbyfzep.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3umvcoend.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3baltxfin.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tmipizes.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aypvhzkp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3ljfjvpgl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fkkizvrl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ltgdesil.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kqyzthux.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wyhgkcqb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ukvxagce.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qabtvkww.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ltdkzycc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hxmbjiqz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lrdgmxfw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhalvgka.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikdtwhcn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fbngxduw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3liijejqz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ewuwszfc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hpsmroig.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eceevmzo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wiqhysox.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3fethssif.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mkoqlkeu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utrqrbwg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wgcsmicp.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3dbjtzqje.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3exokmfju.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uwpffvxy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3yiydctrg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jesblsne.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lnwnxpac.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3souyekae.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3tsfyrtpa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3flikbnny.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3scjdntpi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qkbzpdct.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tseqgjwc.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lbiqfxjs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qsdlmigs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dybinbjk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ifugxsun.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3lgmgbblv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3joxrpfae.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3zedhovgi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3debnxmsm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3bzfojgbt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fmkqfqpe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mcwjqzqi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ljdswbdt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eylikfwf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkudjudk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aklnnwyw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3owliuukq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hcpmimzv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hvcajkox.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3eshxpbqv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ahhmsxpq.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3yazdfxin.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dpajzcvn.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mheqfgcb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3estrfhnj.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xfyfiipm.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpaphczl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycyxhprz.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vvufyuky.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vwqkdmoo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3omrrwykp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zjfwbtug.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ujpgsnzd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rmsbadrm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3eqodlssu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3orbxsrea.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3busedteo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cnqajkht.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3rddffrxl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aoukswpy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyxtxufw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kfpcvyvd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mpfybwgp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3difpfaue.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3bassuwjk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3bzdciqia.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ldaignud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lcffzoia.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3dmjgspne.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3anjhdrde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxlywakr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3chfismxg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zkcaghox.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ntmfimql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kbnvssjb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3dpbmtlej.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3djbunasr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3lzkltocd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yhuowwxp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3thjonisb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wsaacjaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3odgaabcr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mwrtvcol.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wibkkzwf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3uuupmrtd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eekwkzue.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3fjhfzhmd.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rhcrdtds.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfoxahkw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jfkxtwzh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hsygvssw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3sxftwzjj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3oaigtllo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ffhjnuiw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3ezxgscsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3utormmev.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ndunuukm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxdqyenu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xfemkmns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3bnifcfkh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3sgykiwcc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3torgcfeu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3exqzvvjs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zazvyngx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3radhrkqy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3twhsjujz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tdjgyihf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xbebcrlo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cpczpapd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dirpkbvm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ozzcneyv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wvdzqdty.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzsfrwck.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsrzhjc.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nuclveyd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3iujnwlzz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dwfiynne.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gxhkxiqk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cpfqegxi.html


<!-- 参考信息 -->