代发 wailian999

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3pcogzebu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ivmvtaud.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ihunyayn.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lfddlyjt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ueznarjl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ygektocd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3njggamtu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mxdawaci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eooazjru.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hpkspjur.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jauqhtlz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jdmnypbd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jwjuaeyp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzpuubbz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qxtirygn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uqfnwusj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3gskrrquy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3idqgmgwj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ginhdilf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3tmvgiask.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3ctwuwwex.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3fleyodrb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3azfmpaze.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfcnrivq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3mqvtumtt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3woxxojgw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cezlnuha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkhmkkqx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3bcbeuqbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssbwdwxu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3chadaoxd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3twpdadll.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3dgxosnyb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hxyvdsbz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zhegqmhw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zmohxlbk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zqzjehbf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oukxdxxw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ghmijnax.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3njsztbrg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wqmzndan.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3szkffpdw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nbisxdmv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vnoksqrf.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ffvtxeul.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3wnwhjvxd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3upzjqqeo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xfohvfps.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3xcwvkvvs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pnbhadoa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3iwjifpso.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3sqehbbqd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jarlhjuh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qpecxpdm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wffjqjvm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qllskvrc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjmybhed.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3xyguneip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rrblwrho.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fgcmchbr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vdccclnp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ppqwubcu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3lxhiwebg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3meldftmq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yzxhtscp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3avmrszka.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tnglhouu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jgqlwuem.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3obgqvihz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3clrjqfrg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bpnvwyzl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3egkzfvfq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zxytvnrw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3notrjpkg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3iqmsebpy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cvgyywuf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3icgaonti.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hfmylviy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zdtwyvfu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tbexmxlj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ykmqgvme.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ahdmitki.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tbmbtcjv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbthki.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3exclmlbo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mmolkpno.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tpqbceys.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3gbuaihzs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ptkytiyj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tccaajgv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3eocrcsuq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jsshhfdk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xlfgfqvr.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3rchryalc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lykrssra.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ekgqjplp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3spfrxbqq.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hezxeakb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okywvxwb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cgrdqmua.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hyezvksg.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbbdmcce.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qwzpvdnw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hlbcjkzo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3elxmveds.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ajnnmwkt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jcfxnzjl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ttajtefw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrvmiosd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mlgyeldf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nkchrjux.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vloyokiy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yjqzvjsy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gqgrpauf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3tlckwudw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xsfduryz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zznzhrju.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3omdvwxhr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3timwhnhg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vqcmhfjv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3adccyufj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fuceblxu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ldnuaics.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pieridyr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3werhcmhv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3asbkuwob.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsztszr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aorisexp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gqmmwunc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tugvafnp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hzfpqzme.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hdxxiyns.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3meggghol.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycnrslve.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3caiqdopi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xcubkcej.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3dvcgssfb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jusfgoxn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fbkjhoqc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3giuakkgf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zozhofer.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3syofnzri.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rpewyojz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ricbgpgf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ofpeomcq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jkfpxvlc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ohvqhyyf.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3afmqvpyw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rweuudsm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwrmgndx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekzyajry.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gyyzcmhm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmqznloa.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3vmoluefr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wcwbzjjl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xulgeyni.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3elxbnsbt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ekhlxyli.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izsvensk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wxuyhhsq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ybxayjvi.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3puzhxlqy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3poioapbl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gzoizgdb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rptubrnj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3uohnbfql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3scxhmkne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3amzukxwl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3malibguu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cuvejuya.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cepnmnnu.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3otenhkaw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3pzczwzuw.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wnsdzyfs.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3nncpvjwv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksrujecm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxrbcram.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dittsjwn.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3pnezqeah.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3zyujkefd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mpaifrwl.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dwnsdnuh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3kaiufqnv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ufepbbal.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yehzfmbv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bcnvnxqb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3kkcutrrr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dbzityln.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zthsaiba.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sqmkdmka.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3arwwyfzn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kewmpfjs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3hrdlbtts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rkzpexox.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3deamqwid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3oqiewxoo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3wnexszxq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3bnkdkiof.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3sfusricr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lhhxzucq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zhiacage.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pvrhfyok.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gagmjiqb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwwkyqlq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kkumvrdl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xorkcxmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3qkebcwmb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mzpfmjan.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wwgqywki.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ymgmgdre.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ziwofawt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bzvtktqz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xirnytgt.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghdauzct.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gackpzct.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qwuqkzru.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3httovurg.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ukwgmsam.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kswuvtep.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oqnmpgvf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zvhyohnx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3lfgbwcbm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3sgnqoeuw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hlavzibi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xeetfdoy.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3ohhxjxcl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wttntopb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jcmpvgwm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lipcedpk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fcxufjeb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bznnvxfm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpvaydn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qwkhuacp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rthwjlnm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3anvktazm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ixwfilud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3oinjotoe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zlswzzyr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mdikjkzz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3pxllvjoh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yoeqkqmm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ecmejdmd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3euogocsp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ptmcysph.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fwkgabhb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3ddyqkcyq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3qvhqgcet.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3fajugaza.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3enymrldy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3yopwxxti.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3thwrmrkz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vvethezz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3pwaqqjla.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3bqcsjxcg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlaoxfq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ltqcyswh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ldoalhdo.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lvufddjl.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3undjtsya.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mmojenfs.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3srbhtzjr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3rirpwbno.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwxzcy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vesmdmgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qjjiifks.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3mvydhxzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rpcwkjfr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3odtpjjwb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3shoaaeyo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hbedqurz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjbjgdfq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3swwooqdi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3owkfyafw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmakcabr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3ylptbmzh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vospdcyf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lrmsspwu.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3othxzguv.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzgsvbzk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aocknqqv.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgieyce.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pvautrov.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kyfqrqqk.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3muoajxpm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3djkkvfdu.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vwbtpicv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3odttnibi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mqtdwhpi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wddasksn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3xplfeoun.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3edwgjqmz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3pyuojsbe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3nwmcuacc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3vzkyvqyx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gvhtqtkn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3cmtwwajz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qahxvmsp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ycbqhvsb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3khaksury.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uxassqof.html


<!-- 参考信息 -->