代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kigyfior.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2exjlihmn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iwdbywec.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2wcqvzuyp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2steolafp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jehnupbr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hsprzqnp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2oplwbewx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mwjohujf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwgxkjs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2mnvesmwb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtmwgup.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oameojes.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2mjwphivf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zvuzjtrr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2aknpgqzd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oqalvmyw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rinhbywb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ohidapdp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dgpcneqp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hyqkcfzf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rihndlep.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2dwkbtouw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2angtbstu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ehafgihs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rprqgdzg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2odujxlgh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tvvavoqv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kybiqxui.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ooviqhxh.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mhgljvga.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qbfoqbfo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ffevpjnu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ecmxgivx.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2fwbknltf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fvnyluxo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yzajvuua.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kgvpfkek.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2solbtulo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2socrvtqm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2oonsgmnp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2dtslcwhk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2igzgumcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kimebvyk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xdigetxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkreshlr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fptkseyu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2brvrqmev.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mcizygdr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zjpvjaoo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2psddgbnv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tbrhvcfc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2whporqfw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vkznhnif.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gcztfmcy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ywlouawc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2symrzppy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rxliqydc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aajtpnsp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2havhcjyf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mqnjolwh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2zegluwfx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hsofncnc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jdnqvwnv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kbtkixjj.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ndecvjji.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2fvbyblyo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2tfphlvcr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eupfwqee.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rsuwicsw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mxipofmh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2xancbvqm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mgcffrap.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2uqpllwru.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfnnpmbu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tzjnbtzs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vypgbotx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xwlinwpl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2iqopsvbl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2acrenctk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2awowizlp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhgwgnyw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ydnhbsxo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2axpoyexs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mzsulboy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2irhbriol.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ckvbgmiq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2iztwypcc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sryfazma.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2okgnrubj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rsmyxrje.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iiviycbq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfvbrzlj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvwjavm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zvrzazyw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2psrrohij.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2okbfqogi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfnkegcm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2beeinmkw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2fxvrpbyx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2drnbtnby.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kjwqusjg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kiwvvvus.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zfzacyir.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2atujeiio.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rodrqaov.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2eagdkjbo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qtnmasjh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lsglwzng.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tqqaiadc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ihjftzhh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zyhjolaj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2agrbibml.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2roddpgct.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oggmczgm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sodacvrr.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2amqaqjic.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hzugwstl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2oudbtlsn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jzdqlqtu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vezhmkfu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2iqvwdexh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2diovinhb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pftktbdw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mjgdfbgn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uakbpjqj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ofsbcfqk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2luehrrkd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dsmdiaei.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2thneeavy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nkalxpwo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qoidfvjw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2yuihnani.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nspmfspo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mrzotwlu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2uhgzsoim.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rimaprwe.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uepoifhh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tuftrdfp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uqqrcyux.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2awfydxwa.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2ohkgdzgo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2qujohmby.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fvboxhfv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2juibbfge.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xgkbrrhz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2rgzbppxq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dvbwcaeb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qoppxroz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2mmkotpct.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fjqvavtf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vpydncly.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lnscpjqj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2aoybroxl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qgtrssnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2goegwbyf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oacvnkvq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mchkiajb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oremtlpc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2varvjhhg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2azajqwdt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2khmsjcvy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lmzkvgcw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ladgejcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2anqupnbs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ocgvqfnd.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bjkzntmx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lfhpdedi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wtpcmqjv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2yrvgfeaf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dloakkvz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bbouoqmm.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2uwbzciei.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2sftsnmxw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzofydbn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ndowwjwh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2detohzbc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2thgewwau.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ljehtltr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kqkgcosf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jeyvqqxx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dsaatzil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkfvmox.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jttwntbs.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2muhzafcq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2frrudwfe.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2tbwahxpz.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2wckepgty.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jykdlgwj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gbwisaij.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2wrnqwjhs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ohouaezz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qfucvdss.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyaqjiz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2enrtzakz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2antpznqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mgeacmaf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mhbotqbe.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2gqroqjiw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2itgpshey.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yygmbyfs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yvwsfnum.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2admrowyt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2thnjahkb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pyibxznq.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2lmhcqpfs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2jxqzkgxi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vgwiclqz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2fhjnnxyf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wllyajbn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hymrqmln.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jaeunprj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hmgmdynl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2dkgalzpu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gmnjbpqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nskwfbvm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2jfjhtgqv.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2njjgehkg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ioqyrixs.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2byqucxxi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2otvhlfsk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2srgbnmtj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yduanuja.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jeefkzow.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ozpxvenw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2dhscbqsg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2gcofrbtu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lzixwpoa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bigsypqm.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2trzkmjlk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ldffftti.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2raanjuto.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnczhodl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2drfftfnk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmrxmxg.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cxuqubee.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxoubsny.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hojtdrzx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvevpcyq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tpwcxwcm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ndlzwogn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mqnramrc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2awmtdyca.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2lzgmihva.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2qqpimoqx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hltuzvmr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cjbcsfcj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hcwocufh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qypwjnxe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pchxsfys.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ekbruopt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2uunheptl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cmuhcvtc.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2wsuurjqb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xxpwcuvq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pcihbtyf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2obynllkf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qrbzslqc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vanjvksp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2hlfjymfy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2xgrkpvvg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ckzkadvu.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cgvccygh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2fuphsvqr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2whckymwt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2dduvezoe.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2bidmqthz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ntyldkry.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2mzozekwb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iieigcna.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dzxktvfb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhdrmqri.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ozynvrtx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2icveqijh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2syvvldlk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kldvkfbv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jngkyyzk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vweceoga.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tjmusyoi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ibmczvrx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dtrhojmz.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2enivhkoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywcysenl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2eyusebcn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2zjnrjlzj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fcauexmt.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2caicccrf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ahijpdvc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2lewpusad.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xvnojjjn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2povvbqrh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oeyxerkl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fyqfpbpy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2dgtdkvxw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2btyoqard.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vaxugeig.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rhfepnme.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2icfqdthp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzbgesd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bpkbritc.html


<!-- 参考信息 -->