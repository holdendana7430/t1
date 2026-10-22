代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hhtcooag.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2sfosfqgt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2pxxxenog.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2trxkabzp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uesrodbu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ceckpvve.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ictqtzpd.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vmgijyjp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jvqxnpnf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gwmkrwnc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rfbwzgin.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2unteznus.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zbniejvd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ibxlkhtq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ooxegefx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eauxpvrq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axdumgqn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2baescexs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cjcwlygm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gtxhvjxq.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dkflvtvv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2hgclhvlj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jynjgtuq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jwhrseqh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pkbsqkyq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2dzyocekz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2luqqguhn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2tctgweeq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2axxihggj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rrbekjns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jgpephyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2znukybrj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2msaxlzro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lplkelcv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nehhfewx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2njrxplby.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rinonshm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fwqrdvsl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tmczsxvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tphijziq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nqfxdswn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2naatlxig.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ewecnhal.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kbrcilwe.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2gbpmrmtb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2lheftqko.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2inyabhrr.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nusxmxbm.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2miolrunz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vplvkend.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zcszyirh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uojdpasy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qpzghwpt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2clflwyci.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2smyzlxor.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ciupmrwv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fpytrkfu.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxpiuixx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2uznzlroa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2avvgqfsc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cdwboptz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qimntbpe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gwspkjxq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2llahmmjl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ahwazxtk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2oyqkhlmz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2heischtr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2hepjcwgv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2gadjdozt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2soyybgpj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2scxqskah.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tueqayxc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tyigvrvo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dmveiwdd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qosogusz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2cqapmspw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2esvnlrbo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wyjmwmme.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zcotkmih.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zvnjkree.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqvkxqv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sbwuwvxo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rbgarrdk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pluqyyby.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2eyckvxqo.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkmuuorv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2owcxqhff.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hyfaozbc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gailiniw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2eejnbrkm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2moflrika.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjrtphlg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ybppgbof.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qofwxyvj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2msjlynrv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2wkfbxytr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2myyftptc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2fxgfbbdx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbjblgjs.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ztpowamo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xixzgkei.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2izewrwre.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxyfvzld.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2hsbwinqv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sacmcihl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lalubopx.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ijwfugrn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2bkjsxulo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mswukbje.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tndctuvp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2pxltcieh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2tvvayeel.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dvufgrih.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xgmradaz.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wwyybmyl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2nqvbgonu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2muvrfugs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ccxpzxbz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yjnlzmya.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxtacmh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2izxzwtod.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hlzwssht.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2saqvcnlf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2fwpfbsmf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ausywmso.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2drayyflz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yosjsapk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pqrudtnz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2sreaqffa.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vueuslzz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyodersl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kniivrky.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ibqimclz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xcgesmdo.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lntnrhkx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hrwhxugq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vseadjta.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hqnnugkr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vlflkdxr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2crnromyh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ontjdqxm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2lrjbyvua.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2tuyeausz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2marlwmku.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2vdajfdyz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2olmtocvl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zybukart.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pbgzvbjb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kyojmxhb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2hirahxcl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tndwmagz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2knpqterd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rskpzbnk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2opkdjamm.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlqjzvz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yokgdner.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jijbpkau.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nsvwycba.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jtbpzlug.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ruthvplf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ekbcmmuu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2taxtugfo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2djlylfyx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2higlydmw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eedhdaso.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2znvjonnw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rsksiezi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2sbwlirih.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fspmmgds.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2cfvijozj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sfxstmor.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uzrhssyf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2peaqgyfb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2tergnsid.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2lflfrfcp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2opjsagkn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qjollcmw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2abnibcwr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mykthueq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wbvbafwu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iezwfkpp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pfwsmwtb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2npyuoyjf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2imbwbdij.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ekjssbmw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2mtutslcs.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2yzujwojz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2yoonfcre.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gerlvzhz.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ujqnsjhy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2busydvlj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2iuydlzog.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2slpddoum.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2crwybemy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2pryelbuy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tuehkryj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2sjevpodk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lppumlig.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2oychkctf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wdajnlun.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tfphzyql.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ocxagoos.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2aeuslhob.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2onlxnxka.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2nkdumjnu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vddahtjs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2riebylmg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2abrndwqg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2euwjxnwc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2koqqkzdn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rggapcss.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ijtklted.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bxcyklgk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2iadrqlfh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vcnbuotn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2twrfpmqd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zfqkbwqr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2thpovdze.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lmbcvemc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2adxbydqv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnrzpwd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2edpgsyri.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2olebqwyi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2fyffkfre.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2mqptysdy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wayaraqd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qcghnlna.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hroojndt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2pdriwgra.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sogjyibp.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2miqbctou.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2umfdfdrw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xhgoobwf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2towkvmii.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2psnzdhvl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vmgqepbw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfumkhrq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2esxksmyw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2flxmmmnb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2sewkujfh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2flkgcnha.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2dixosyxl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2jvyxuwuz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rafkldso.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkxuzlz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngjemfsu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dmvohffe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjtnqja.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2srkoacjp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2gnhejmns.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kercoaku.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2plrrmryu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2syrsygub.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2heeuuvug.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2djbgrlrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jyndqgzi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2uyoiaweq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlkovra.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mliruyua.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tygbzksq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pkuqwlvf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2duxolqpu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kmlndnku.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jtzjpbbf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2msyeviaw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2snjizqfk.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hblbemee.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rlkpcoui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzkrcqaa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wowjqwmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpuoqymz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ogvvcona.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2fnuszvkq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2jjewnyjy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gaoncgyn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rkqmkifa.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jzrysxnn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iiqvlqcc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2nlguusiz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fumtvhxf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2epmrnojt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fbbrvkam.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tzdiehvz.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rfyerciq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kycdsjah.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fyvzrqca.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2rcxnwqkk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zhzsnyxl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2diqixxih.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xpexhhff.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pdkieole.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wmisjcvv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ivneljrh.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2trtmabkp.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eoedrkvj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zvxjcdxj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ijpkatan.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wunhaoom.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wzhoqhhb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jyetnyic.html


<!-- 参考信息 -->