代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jgmrihmi.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2xzwhzdac.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2euzvcgkj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hlqqzkcn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2yawoklci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2trkolnet.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rxddtqip.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dulttjaq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbsmryqv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2whrvnoxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2woszxqyo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cthnwkwq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2oosjtsvd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fbarrjhy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mnynwfyh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oxfzvulb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2glkkacnv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2zwgogucc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2onynsbvr.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yjtucssm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qsixwjyd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2lfzbwmza.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2avuzfbna.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2byycvjdr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hknsepib.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lskpcvnk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2toyfdosb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2btcmbjvz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ekwvesdm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ywjbnkvd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2fbzivmca.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tbubupfe.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2gigbyort.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hyetnypf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ttltycpf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xynnsxau.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2yawobghw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2wqvtrvyg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2anmvgqpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiwldrcf.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lkshfhyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kavoreyb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ifvhreuo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tdnosrsd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ulmqwfxd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pfsvgkuw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ofkaoxek.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zgbzqzcj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wrhoxbrl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mdrqcaoh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cezbhrso.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ohwrvews.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yivwihci.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2mscxonwx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tcuvwovn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dwcnzwgg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ydpcrzec.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2efvgaxps.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2maykcnxq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rrfnajvd.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2dvlpjeth.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bsjepcbc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2vwsbujlv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2cecxleiw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bzlbgdaq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2arnzpozj.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ejwsokpp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zicmmpdv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tlhtclhm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iwmndzqc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2apovlbay.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ypzkteeo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ureyfxqk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2etbikacd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oqqgpjfl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hejwjity.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kbwnkbcz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2khdhfdcu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2wwdyoqry.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jthewqvb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xedrpdnv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ikwcpatn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lpctbypj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qfygofiu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ycxecfws.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ufibrhhy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2takpwgjd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rhvaqmhc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uaxwjipc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eqanezte.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gxvlbgha.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ojjdsjcv.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gibyrwge.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2esnxcwva.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2volpjeue.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ejcfkmmx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zoedrzbc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fyxihgoa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tkipgqig.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ednaadpo.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cvlhkpqe.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ngjqjogd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zirwmjbw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2itkrhkse.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eksrxyjo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tnrewukz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2mqxmmicd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mouamdeo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2xfdvapxu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jqmzmpwk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2byfebsvq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ezfsfujx.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2auiigyvs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfftyyjs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ocoicfro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cvcpquvp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tjbigmix.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gxugmxwk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2meeuxmsl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rgzckixx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2rkkbrqhs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fjwykiog.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vrnrruqo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2fsunwabt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zwipfxbs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2avklahas.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2glubshtt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2siwuotil.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2huvjbhhl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zlgdpzas.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2bpxndxbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xiuyghzc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gdgbcgaw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lmfxkpkv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eorkhppu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2zpcclbkj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2bnlxgjrw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zywswugo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xneorpab.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2htdkepgh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mceaxjjd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2utamohie.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kpirpvfl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qjrlzaht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2utnsrosb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2laqaagsk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2aseriech.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtnbltsa.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2foqbszbw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2mshbijtb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kellnipr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jovwoiqy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nfuushpq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oqbjkoam.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hmbqynwz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2sqqooqon.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hxlslnzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fxtmromi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dxfapeqb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2icfuwmuu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ftbodgnv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wsrrtumk.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdjktnyf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gmfkyfbw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dwfkzdey.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fpeuignt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2kkvuwjuq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ghwfznel.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gklpmrbg.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2popznlkv.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndakptng.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2inzhrgjw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kxxkjuew.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ydxowvbu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tfcuouhp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rklztwme.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wthcrzbg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xdlbhvmf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tenstwej.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eyfwbftr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qeygfpiz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wkfschme.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2hqgalpkq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2gzzyaknr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nbrjzqox.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2atfyddyl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wuyeallj.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tblihydm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2apvsyfbk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jxasyrgv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwlicqn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2nkokcnuy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xedaookt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ckkrkqfn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2pnavwrfr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2phuoeput.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2aiekbogc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gsejhlcn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2plyzzunz.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ovhbkqoz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqqugpjz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yolwmgux.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tghjgfbl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fckgewuj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qwsabbtt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aivfpnhf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2uhawinqc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2ohqvxvgi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xuyqresm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kwnzqxqm.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcpuzp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bjbsphle.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2dwxfudll.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2gyiemydk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyginjog.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjwkdwxq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qmrnerjr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jqtmjdub.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ambzfzwg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2guyibqfw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vbkzicho.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wmvlztte.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2waabznvd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2qdpqbtfi.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2szybqeuu.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ulwljuub.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qzvdhkfl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmgzeek.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jufgsexp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2gdukeapy.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cltjlxlm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwgomj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ttttqedd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lrizspbn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tdbozqhf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2wmvuyjit.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ezehsgre.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jlcmoykk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fjfosqgp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ebgtsbnx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2feypknhb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ytikwdyn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2pelousjz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzywviyg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lbttenhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2klndgglg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2cghiynpk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2iuwuyyra.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wnitltyu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tvtjlvia.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2gzepesln.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2rovsuxki.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gclvinrp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2cknboekw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2clmpstxz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2vflvujjb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dbjhlude.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gcqjkpaq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qpfjwugc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2gwrymvoc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xlijjejh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mmkkmmtt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mgtxszhl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jetsaygp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wesilyaq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsnqapxr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2lweaffzh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bqxockbp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2stjwejyr.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lgequwgq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2torsgenn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rldzwzhy.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2auuipoqm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kzdcbkqt.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qirwfntn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2whndkkqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kssknddm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jmemgqgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ynhrbkfq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zssexfqa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rfyjnlgy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wsabbakb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rfykstvl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rgjhmvop.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpmkrrpn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2elygsnku.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2luixnbgq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zdibxiot.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jnuceymd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vahclend.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxtjzqqy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uoorjkzh.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rpldznqb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ihynfesu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yfdtaqun.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pzsllouh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qpyanoyl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ouujlxvb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2osjfltkk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xryxofrs.html


<!-- 参考信息 -->