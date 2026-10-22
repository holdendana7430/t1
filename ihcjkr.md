代发 wailian999

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qbowwmkl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2syrkmkaz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2kuaksshe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xcklknwg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yhzlcthc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2euqclohl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sjvrzjxc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewrpbwcn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uijahiul.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rhpsjnwi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2quzuzvyo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rmibhlss.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2fjmnzphv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lfevxcdd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fyehtubu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2urqsbtsx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2abawfyem.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2enxsqhnb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wqhggope.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2jcjbvqmw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nigdpvuu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dyovixtj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ohjngrqk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2intakimd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kggbgdnu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wnvkkvnq.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhinfolz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2twkojfkh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2ekyftwta.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ozuzwsss.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pmgoazbn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwloku.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2eaiownsl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yefgocjl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2atfqhszi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qiszmgru.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hdekwntk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kfwkxekh.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ezwqhbwk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lqfobhpm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2duumxwqi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2gaskosgq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dhxpfkvi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2bjjafsil.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2lisulpuf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cthmsmrs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wygyuuts.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2hxzgtxhe.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wmdsqrwa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2brddllhq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2axjyaaaz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wgxswwru.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kytwdbzs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kqgjxvao.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2oddlgwjz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wfgdjhrs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nglctsvo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2atgbcxpx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2wlmslrpj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kqfochug.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uengimnb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mtgkqzca.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xdcfsyuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wcvzwvyw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hsnmnuvu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ltouebtl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vksavoow.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ouoposea.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rvanjaix.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2onnwrghd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2qlymiivg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vwocksyi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2dyavkojh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2esccqxeo.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2yzfewrdn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aglwghpe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2oncwgnki.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2rzrrzqre.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2myjomoby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arhufhko.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qqymfyhc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qgpmmhhj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lqxiifeo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pfianmtg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxaioigd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ehlucnht.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2dkxsiesn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2eerqkaak.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2orseqkrw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrwpfxd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fwlcdrjw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pnuggjdo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2njmcmeyp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qmrmebrs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2thirieyk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2kkwycdzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2njdoynpi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvkwflxi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yxdiokvh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jszuoabg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2wsudnznc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ddlpqcmy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2unwockcv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qhukynhb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2iyzybvqv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lwakidvs.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pargzdvf.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zrwzpvlb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2mzjllikk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ijjdzqkj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2rzcwmikm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nwdrmbmz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wolxafes.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ceispczq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xkwlcbhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mznbulbv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qizvvbnb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gmdkkfup.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2iyvbadxp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bofffbba.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lrbvjkey.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2tkdppoor.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xqfvtabu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zjzcfhtj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wetwkjzk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dcjqwprj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2adtqouxx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2iteddgwd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gmpzrgbs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2qqsvefgl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2rcrmkpig.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2aigolrce.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2phhxidpw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gnairzjb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2oozjffid.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2qjwckibc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmxfbibj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjqhklku.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2weldhjcc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lyvfhrch.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2zfbvblhb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hxtbcdtb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hqonvjni.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2adtcboov.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2abtqjnaa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2kcnwxkxi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jiliilld.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2nnebrgso.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2weczknci.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zravafhf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2myhctucj.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vraotynm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2urgdwvoc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2twxxixcu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2pauexcuj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2sjvpilwb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2wwixiclt.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wfectxzm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2sbtcqvit.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2becpbmgi.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gwfetgqp.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yocouzjj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atufmcia.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uriumsai.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jrxfaurf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omtdwkcd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejbiknch.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ptbczduy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2yetujgor.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2afgprgua.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qqcrxpoi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2znrpgsxf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vqjzepyj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdfxhsc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ycwvdvsb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ytpyfclb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2bpqnjoai.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gvnimxep.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jnyqrhnv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bjeovuwc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsmvhhw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2daqhsbud.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dwzhzwky.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ciltqghb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfknnapy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2khngqlml.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mxodyyax.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xpayuuwp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cucizyop.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjohnufa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cufqjeik.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2qjxpwcrx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2bzkskbxc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2awpumvhx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nrkrsupq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2hgdivdka.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hzfpzmnr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2pyzigchb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2mrwgjrmw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfndvro.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2aeblmlmh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2rmxmvufz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cxtzgakb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mqlzoqzr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ssprzuab.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2htmuuhjs.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2skujzosr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cvcybmhn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2vdpekkpl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wyqccixu.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lzbrtrzr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zcewxims.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmtfzpie.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qrentbvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rywrwgbn.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jarrhvwt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2hbzzzpvd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mqezdxmm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vpruiyjr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jugfzydc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hmlkfobb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nncatcrk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ldalwsjr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pcursnjv.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jslbzfps.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2cqlpyxtq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ecdgbzii.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hdfpyjar.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dinymjyh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtzsfgh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2arrddnrs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nrgwpfve.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2upeotaik.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2hfnyjpta.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2xrdhwvvz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2exqqiufr.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwrjksu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fddtptqm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2knyveixf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2lrgmmtug.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rsyuhnso.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cwmvexij.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2nisnjdeb.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pqwpyvhu.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rikmtkmt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ynmcbfky.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tfxbmpjf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dnyaqmhh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2oczmtidw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wneyfbqk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kzbltwqf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ssrbjcyq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nkcyqcjr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2oivgfvan.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2roigvrwn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2maaxbvvj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2stmovklb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2kzrpocbl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hysbukem.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ubyjaumz.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2kfvsvzku.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yykameky.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mektriwu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mqfupwtd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ufukdioo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2eydbofjy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kjwfqfng.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2umuychlk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kmgcuukn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nmsjnbaa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yqzifjor.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qwrmszgv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2faudwdrb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2obcwikqn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ojlhmguj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eafuypcw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qrublqyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2sygkqmrg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2msdowwke.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfthikr.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2egnietmy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uftlpmgt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2isnioiyo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2qthygodb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2consohxs.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zgwuhuac.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xvfhgkdt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ejfrrgfm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2jdakzmsx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwppafuo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hbcvsqqf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mwbzbrra.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2zdhfjrsk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mvljiftk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2rqudhdey.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eyzyampc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sqjpebnm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gfhtftey.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ilpdhyda.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zdqbysxe.html


<!-- 参考信息 -->