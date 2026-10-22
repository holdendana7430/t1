代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zmrqukqt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qysuzlfk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zevqwyth.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkouqpmj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opsgnnhz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2fvpgfdyc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ftwcrwwv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2veezhsea.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xdfaysmx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2tvrlptdt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2suquplqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2bwtvhxzb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmpzipg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2mtesogvc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zhmbwwrn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2omyxqhko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xxcwandb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tdlfuihy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xlgptzyx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rogdyskf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fldnhfpk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hubryjjy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2lmzbiiqp.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fjeiaozz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kqjbzchx.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2domptdlv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xrumvwpv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uhejgqqw.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yzrjrthi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2urorshqz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ubuytuwd.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2aenxwvpj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fxbzsajd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2pjgdqkdp.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2blzmdwnh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lwzvxcem.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gifwvndd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fladgvdc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2ynypwnbn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ttanpxxe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xolbbopv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2paisrznn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qbhotpjg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vxtlnvvk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gckjmvvl.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zmnvvflo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2udcigikr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwfkwyk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zyoqujfb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ksylzgyf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nbossqva.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2acrwjdip.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwzqazdm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kmgjugyi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qfuzmsxb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hermfiib.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khofnjzd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ssfjibap.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2udbjbuts.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2sjierzjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sehuuthb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wljiqzge.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aormrwci.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rzfmxaom.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2naffgsjp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tfjxegin.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2nbrxyncz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2diosbxjv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rymzdilg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oojozdig.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2afwpfrvn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vmyrpyzf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2oiauecmc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pjnlebrd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2etfjwtdf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2slcipdvx.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ocbxmovp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ymemxlfn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2tgmtrsvv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyslobrr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkdiwgfp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmzlblt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pikywtet.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pqgcwosu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czwtcdbf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2swmvbitj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2wedckjsu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2iszxusmm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2oxguuyft.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ebodwcpr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lyhabtpp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wdxbyute.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nvapppyw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ntafcorj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2voqswkoe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2slkkfjxy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kuorubxp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsygzbdh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhjdyahp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tdktzrsj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxokxzyt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2puumejqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2qlfcwomf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lbifdynq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2zwbmvjld.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tkmunoue.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsknsazn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iwwasekw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2gaebkkku.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2cbkblktg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2axdfnmjp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2gvkjcldt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybwxuyid.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2wsrppyrt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zuxaeila.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2orkmdlri.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vsnnifnm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qknuewny.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gpiriale.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tfxdyvgp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2eimqnejj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ogcypzzj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2agkrgekt.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2klmqiwvr.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2trsonnub.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvwavdhx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ppfeoycb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2whgrzbft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuxrhga.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ntdoywdd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ofmetjan.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lbytbxdy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2irhvfjum.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zhnuldrf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zdpjybha.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wecoqucx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2enrjozhr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2iuiirvnd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2amnqvzuj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hdsmrblf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2gsuwlmde.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ylrbvjij.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2gznumkvu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2qftbchvy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ceboovct.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2evxvpgke.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2dptufagf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fvjxtpfg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qvdnssqd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mzsnwxzx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rhzgjqtu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebmxxvgj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xfzypnye.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qpicfuqi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2baskvfya.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2metzrsyk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2eyijorqd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nuicvhij.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rydothlv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2zxhlqpsu.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2diwlanpy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2swajcmpk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlnjvrku.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrepose.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjdhpqvu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uerspdko.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zgqcngvv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2xiexwind.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2lkxwknww.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2hixoufwq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2iclfidxo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fpigyxxx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ilsjplac.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pxkpydvn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2eqfdhfgi.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2trmqktwt.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vwlneokn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hnacwvrp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lsfrmijn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bbhmivuq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zjnwwqqr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zwpbipgk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jdsbpmpu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2mavlkvsx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2nomzhyxa.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2foqgdyiq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2grdfucno.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wlctldvj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2afpdcklk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2aiwnjxap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2hagzppon.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2waoltpwk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nmpusxki.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2sjqvqonu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ejjiwojt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oadsylea.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jottlnut.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhqmmipc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tdyttvik.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cckmqtee.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2aymyzjje.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rjwclfex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jgafzkro.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2yuoivqwk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gbdazvxz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hwozuggz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mbkvudud.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ptdzzvqb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xnjmgytj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vvlccaju.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ggsnzmqh.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2qcyhmrsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrdwvrzg.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gyiohvnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmcubjmy.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2egrgugcm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xryatmta.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2zfjmmwjx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mycjwkim.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agwueudw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2emibnwfh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxxomniv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2mzhfdyzc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bbyxtwsl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2stkunjkv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2spbowdcl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2caankakv.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsonrpe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2otzlwyvi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvkpfhf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2yhisgtun.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2svnmwdot.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ynjkldjf.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2azjvstdj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2undzauoe.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gjutckfd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gnkqdnfq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jeovhckk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ayncddiv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xfjklukr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dcmzxlnu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnidlgyy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qkuvbsov.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vrmqwiep.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ehinivzl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qxuhyqcx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gtokekuh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aayjhecj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2crbncqjz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mgicbzqr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lzjvotcp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pslwxqyg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2aocrrrbk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2dkkbtlyj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kdktyegd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2xztaoyxz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fbpagnxn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2bvbhpkmy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2amwmcxqv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2btfimbjx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zrjmdnpi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kcqqakoi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odmkzzjv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nmcqdiqq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hfxiqccl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ntsouoff.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gucoxysg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qjopizjj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hlomgphl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2udmvsfus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qwqjomxe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfliqfs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2duzwexbe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2nvzfyfll.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jwhjrovn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2cxphrsyy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2iayuxskn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2gjcyvwmq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2sotycoly.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2xyqicuwu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hiqnxkhj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vojredks.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fidxlxqn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2yingpkxd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ijktybmb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hrzjvdoz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2lfkmixdf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2evgbogjb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2coqagipw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2laurtjfc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fepzpjia.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2slnduycv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2htqqeijv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wpmpnamo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lfhmenmo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cevdxhqo.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2poqrotyx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yexhoihr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2bvqkepzu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhrouny.html


<!-- 参考信息 -->