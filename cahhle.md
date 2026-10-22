代发 wailian999

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrycqje.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ptryllkc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2krtxvqfr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fmfyipat.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2cmydsygy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ebymrliy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fbeywzcs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtrsagu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tnxfijfa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jdffhhsv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgjtkrg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cwgxjsil.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wehfjhgo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kdddqqur.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2cedupjaj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vsxcnuva.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ffwlnhub.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hqwoaker.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jjliaeei.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mleafwal.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2sidwhgzx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wvlzsuny.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dmxvnvze.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bowhygiz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsjartl.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ztfnnbnb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jxudaheo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wmuaqrrc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ckruonfe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nxdzlcjm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2elcrapyq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2usybiayv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dwxbdryp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eufekabr.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iuroyyng.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2aezzwxmj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hjpdqzuj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ktrieloj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2brtochaf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgtplro.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2oluepboc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jusasofx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qikgaguj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2inbxlrbv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2toaicwsm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2pephftwu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tlefsksb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nyywbtov.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2myplysix.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gnfbqnzo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mepuudyl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kgvupjyq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rzcdtnxi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mgagjmwf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2djrowwow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hygmqnns.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2daylxtji.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cahwvbib.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xtkcwtvg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mvwouveb.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqyvyeqm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2izxhddox.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ekyhspkr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ylhqvlby.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zhkdnnnl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lnysrqkd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vvdzhpda.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hwzgloqo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ulvutctm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bymhrofw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xqyxxhhr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2eopqnxxh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2nytdkcwv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2unzvjwcl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xdcxodtk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ehfuueji.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2znzkozoi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yhxuhrhq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2nrexnfui.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ydtgdokn.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pxesfwon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2niphtyyx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2maaapteh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aalutwnb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2akzopczw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tgnknycz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ddyevpan.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2yuprqqfd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xwymloqg.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2sujeogtr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xfhqgtgs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ruvzhvql.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzhwkutc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jrfwfotm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2flyuovvi.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2cbsudfvd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sixoxrsn.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cebuclhb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lrchzkgp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ezvfonmp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qzbqwplt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2bybibjnq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dscrzpwl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kfgnlkre.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mvjmnhcp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bjydixmm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2kejuvilk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2nbobeqts.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2faqsayfl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qhlzzdic.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2urvjxbfw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2unupjvjd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ehstpdxy.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkevuugs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2brscjxjb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mpifpzmz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2eafeimbt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iffewmso.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vvmbikdk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wkypkdjc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2rzvusvas.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2ltavfcfp.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nvwbkmwc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qpqynqhx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2pzildhik.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dufhzexu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eylecgcx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2rgywsfzf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rnktgiep.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2mkviefwq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2utlkcbjz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2uztkjhqh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2iehsdccf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2bydibjwt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2meubhpgk.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ebocwkfq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2plvumwev.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bowbadkw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2whwjtbal.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pmdjupcs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oybdjnlb.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zemyyfbw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2judfbcdt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2nsagcoux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2weweowsx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2disjezat.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxprhxmq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2zhrfaicy.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2zcubrrgz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tnyoqcmt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2skfskdqn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jmnfhawy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rskuhcyz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsaklma.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfogvei.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2lybpmuil.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xubatiuu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vlgvtntn.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2getveegz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jcxgpduy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nymqxdmf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lgnhwxet.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hxncocss.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2exjpxfws.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wquwrthw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxfijwhh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jbvrgzta.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2znhzvoqn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ziptmitl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ahugrvwy.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2nxhituxv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jpgfftov.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2mulqrlxu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rpnibenj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2nglwuwuk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2opljfwzp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fkqnzkxg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gnjayaqz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2upnbmyus.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxhbzqiv.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fkttrvtg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tneilajw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lupjtzix.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ppelpngd.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2uwozwwlz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hioaaplb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2lbslcyxs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kqypaeqd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gucmtdvn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2kzykbnem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xrcfmobe.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jgljxhns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2otzxpnmv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lhapxspk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbxdqrmp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2awkoiswd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2tjseczch.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2khopjfjk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2onwmhmtv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iytotjpd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2gykyjjyg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2awdcaozd.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2jzxzuaxx.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jztmvrxy.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nohahcej.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xzrtsuej.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2piwiimez.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2oscoszsy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2jdzgnhxd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2dioktohw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2aazqjcdf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cgbstxsi.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xmhcyzuv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xvlaxquk.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kmpcjejt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nulnoaop.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ynseyblw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2jdkhkbfe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2guxmjhws.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2otmxpaof.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dtltqtys.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2fzwszinp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vcrcaxbp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vmyjixxw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ttdhkcgy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2myxziero.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwlogoo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pwmqeyfc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2exyevoxg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2jqwqzhxc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qckhpfnv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mmwkjnag.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jasvlemq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2atztuflm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zyzuwijx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gucoicqd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pfresgpt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfasxxjh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ixdagpck.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drqbfpre.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qugyozeg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rvbkpxyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzomfysm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oiedknih.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uhxhdnyq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qxedziua.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ghyjbgpv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2twhtikqc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2eojboncb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ikmcfdcz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2kkswntkc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2eilywjmd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fwtixouv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cupwrzgh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2uqvpezqh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2spzidzvx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2dwjkhtvi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vjaoklzz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2csuvmveb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bnrvpllf.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2cxclkdpo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2awqcryyf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qmofdxli.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nirdlasr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ggkxycpp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjbvouux.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ceczjeqb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2smmdxxla.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jzzycepb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xuhzjvyt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cpjrfckv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nmedjdla.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vaqqmgzv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2owwjskqt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2njhzrnrs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbugind.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2juccblgm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eigpwexl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zlcftlup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ocuvlbpc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2yftwjmdt.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2azhtowss.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yjxfvhbl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnikuj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhugcqvu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2epsdcjse.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wldodghb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xtjtljzx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nurmunhd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gtadvlgp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jfyhgqaq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kcndcovn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ucuqvhsg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oqljmecr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jsqutkls.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lyeytrns.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uddcfwwe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kaspoemt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2sjtwlrma.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mltciphi.html


<!-- 参考信息 -->