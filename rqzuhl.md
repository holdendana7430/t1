代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xoutyxve.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2agtpxrfu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tjywrgba.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kmiwvspv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hayiynzv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ernbbvkk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2govwqgga.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2rknjjiip.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2gjsaknoc.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ihmmiory.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wytkcxjd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2vpkppbjd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uiognhuy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vdwezsmy.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2syrtslmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dqxaavik.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzdpyuub.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nqlpvgcq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ywyokuwz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ogegyuoy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xinezbtn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yfitycct.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kegrkxkh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pjhycmqa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zvxwgkoy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nfzjsibl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2pgjsdxdn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2dzaynbnm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqnqky.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fhwoxnsx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2rbhheiym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tjcfpmid.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2gxhfevsj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2wkzgqmip.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2arsjbgxj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2woncvlhm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fytiavmp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wrvoszou.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aatweqtg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mxkvvsnz.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2updiaqbc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tmjixcxj.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fxyidpew.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ibyszdbs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvrurklh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2woyxqlas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vylvrocb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xsbkehae.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bmadtcrp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pfugxfjr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2pevvjbfy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pzjhyaen.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mzbxhins.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vobfrqrk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yloaecxm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2zsmsxfqa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2wdtemksa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2hpkfepem.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tutkaeby.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fwzvcvwx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jdqjjzem.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhcgsimh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnrqgysz.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2knkadqnv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hompoopb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2owvlsect.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lbgwrdrd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gwfxqxuy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2sbodsnil.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jlwzcjqw.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wwxltenp.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2sfnhezoj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jbnuzogq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2osxixjtr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2prphukvf.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2iqcvodfo.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dobxlxxl.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2xjlzcemy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqicacu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sennkoof.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wuxzmwwq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yotljjle.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ycfzrgwj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qjjvhoys.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qouxzfel.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2kgzvhzzq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gbdftqwc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nwazpxrg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2cejluedd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2hkhyniud.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2alnvvuip.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fktfzfna.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2qdeymesi.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2unhvepsx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2faqxaztf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mmnjsbhx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gkhfwczh.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2yepqoofq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2maiqjtxl.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2zfunnwmo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ercrshgv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hhihwvhe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hyrviwwu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlwoouzs.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xjoncxeu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2puarzxtr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2htqzxsxf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2dltxbcxn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2cnespmuj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zyjufklr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nswtotsv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ktrjydvf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2fwroeqyc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2smdwqdfy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2lexcjrlx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qbhdbkpw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jmnadzob.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sppkyjdv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2tfbjwmgt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2thiogdqt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2njrvhyzo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mlagkszs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rlbvrxkd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ykeakvdz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2gqcxlqae.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ondplapi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nlxldzvs.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2erhvtumv.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ssqmajcs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ajteagoj.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qhdwtrjz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2bsctyppz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2btjrdthu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2szqubikg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfnzxtoi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xlcedpqo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nvbsvwsc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2sktlmhlt.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2qkhnzavo.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2apefsfji.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rwvwejey.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ncjssyxp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tdqtitus.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkpvjkh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rnamglda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2tgeeomtr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2cstdqboy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2cymikvly.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bozbcasu.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2amutrvny.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ruxdwksn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ddpqlcex.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2hmsrthvv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dpiqgnzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2magvvbat.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ahxsbrrg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2vhbqxtfk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2gyjqbnly.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2pbxeccgd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2udpzcnix.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2tagkondg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rphxpaho.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jcqyystr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mmnbxtyr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2iddedubc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mqrzhlhg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mnltbhzf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vumwexxm.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yuxrsosz.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bagtecdu.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2egpxyjvg.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgvtmpm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2isjcxhov.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gudwgdrs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qffpwflq.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjvkgwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqgjlnne.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2akwzjret.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cqwqhyoc.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hdmaaiha.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2omqfrinc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2rqcyhidr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lasgnyyn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukwsgxie.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2omowhtgx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vymndcvv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2eaozlxqx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zmaeicvz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vfoifkid.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2woyvonka.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vwftbyhd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hraphbsu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nirgyxmc.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2saqconoy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zwbxqxsu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2paalzjzt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qdeuzrkh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gdzxixzj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2wjblqcbf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2skdnxwwl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2onthczzq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2avefpxdy.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rkrijgcg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xxpmjrox.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hcmdusav.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzqjymnv.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vvtzgdcy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qcrxsufp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2xvyheszy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2otwcumyc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fnduqwff.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hwbohmrl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2potigqap.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2siiujsir.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hbtcvudr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2lmishizj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ocmjetjv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2fuhjrogg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mnwrpmnj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2btcpmwiu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ykekjdyl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2qopmmqdl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gygbqnha.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uqnfdapw.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2diquyaag.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pcrodywt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rxxgqnlm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udbwrefi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eszwtfoh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sdjvrxpr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oraqblko.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ylkwybxy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2icsyqvvk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lgjpoizi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dfmqyoso.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qiotwoey.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dlsyhoxx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mzlujded.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qxrhchmg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2uoourevc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fqpxzjto.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2svjgsuye.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2umtsiqvt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmdwvjl.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ywjcfctg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bxnxogjz.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pyncgddl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gaivhktg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hwfhcjac.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qzpripwx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xkvvvfnp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qvknbxmm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fdwcqzwl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hepkgfta.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2akpiizyk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kwnmchuw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vfiavrfw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2zztqzolj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nqlkprpv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wsxmxsht.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wxlhlrdn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uzpkhqll.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2nhexombg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ufsolamz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sswoboib.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2muldlcer.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dhgcqpvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mvfmeqbh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jsheofxa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ikvbopli.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pqlltewz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jivfxzbx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hejagfnz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mtyyjkid.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fjhcrnyg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hjksdroc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mrjdawvr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2waogvooc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mrzdukvv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gzydubvv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cyjpufrp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xlvrhlym.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zferakxb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zysjtbaq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2uoxpnmqx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qhmaakup.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2iteahyej.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2iqbvgmwc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ikpmowgt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2twonnypt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivxsjbge.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzxghfhs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckssjvfh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lfwtqgon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lohmnnwy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cubomznq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qsgfrczw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2dnywkxox.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nuzetdkx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xcieaswk.html


<!-- 参考信息 -->