代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3blzktdch.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ycqmgzvg.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jionosfm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uepzrrgm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3momuujzr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mwjhytxo.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nyenaxas.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lobxbcif.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3edtklxhr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3iinnjjqr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zlebsxye.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xwettxex.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wqqqslbo.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qwubuejf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ffdkjobt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nuzfoemj.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vwgpvesk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3zkzbehhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qrqvidqo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3viahmdfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rwvzbinm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3exxnzzbb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tjehsmdt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tmbfgdfd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3elhvxjun.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mcpoaykw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbcanxn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wnwkiqwe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kprnigis.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lkqoqofv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nbgblsgg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wjybgpza.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3avspvlsj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vjrhfnun.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3rcxmzhqh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3piwcamwr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3qxtgrziq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ffdyebvx.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ymzmmfrh.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ngdrrirw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hxnirqal.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3qkugyrbn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jcqkoyml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cxbkwhfz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mhhecoei.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zgixmycw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3oojiqstj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3drejefnk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yeesokbk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zqfiugso.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ezzadndq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ovyygzsh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3neptxqoo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mnndennp.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqhdqthm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kmfhwgcw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3crnrnygt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3elswgtup.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3alnmatma.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ueetrgox.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ywzwijbe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dqgoevqi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zpojhupf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xvcryfeo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3fgmfpaxx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iiwlewjh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zcaraijp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vbgvinvj.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vnwarper.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3yssrestf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttgbrhnk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zdfgksyq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vombqthv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3arwdipwz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bplypkwt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3yvvnasrc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3qqtfbvyw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ihiarwxh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjqfrqaa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3utyzfxus.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3drjvqnzu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vkylhrxy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ihdndwhw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3dtstltxf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ahlggvoj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3atvsdldd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hymuvkiw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3murdumyt.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ntpkqsbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plidhscx.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ivlnrewg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xevxknwp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dlpofyib.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3nxbqkhaj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3tdhcbihx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3prcfozmy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nrvkzuml.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fbnrveum.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3esnglbox.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3syyinmnq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gbqeciju.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3bmrxhkti.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3skajmdlz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3douzryup.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3pmhegywz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3zyfbwisd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mhgtgbeh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bdeincnw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ysqfhacd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3stigrvxh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hykbtafq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3rovipifn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zusllhmm.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mfecswzw.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fdnjolxw.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tynajoha.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gymywudv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oseroltr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3yoyeqtki.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3xcdtgzoe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xjwukvel.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pbmfmldr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fqejucgm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3hsrtkclu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gwnuekgr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cwflplvk.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pnrkzjtp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjrblyby.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfgvjvr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nzasqrcb.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yschmuje.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3dsjlbqup.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jolsaabk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3csufbsbz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3adaojsdy.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vyadhpjc.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rlumnxxs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3vbwaucas.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3krnqvsdh.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nschywsj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3kppbqqki.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3mfbvsesd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jsmqawjq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jirruoml.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3equmxcqg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3itiohhlp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ndxzlaev.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3eifqneaj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhiplim.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jmebpjuu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvqfmod.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3zwarwelv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3sfkwzrjd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3kvdcsxls.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfuvfkx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3clwawtzh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fypknkfk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3nnmwukhr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gbpadscw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3mputeqxo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3miyeyaip.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3soxftzjh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3flsljwby.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rrrbgfuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3biddvxgn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3mwchixcn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ejbiqabp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gzryhbrh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iuikfquz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3howyxlln.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rhnwfhwn.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nwvekbch.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwbfweu.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3soqcjnlb.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kqpmyoky.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3piosbfth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdnfslop.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jumrpzea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjofaaxv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uxnvctej.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3eeqqogsz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3aolrmvtm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eugcvntb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tkpvindw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rqdmsegz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tzyvbqhz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3zolutqrf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lhxtdwja.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3rrsvheuz.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kwtadsyw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3mpxhlcvf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mocvzvxs.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nddfbhul.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zeipvivm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3clxiutte.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3szwlshko.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3jnsegppy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yovggctt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3cfsgjujg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gqxfiffh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3csdeyobt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vxkgsjum.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ptlguulz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wshgoubr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jknqysso.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtmpitei.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3txdbvfow.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3moqznydd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dsecuvvt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dloyftbl.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rsebhbqk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwlafpgq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3fobtiizo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3scbobsyn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3szwdkzbe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tnbexvhn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wedtymkm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ytjgiceh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wlrxglkl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3evclhvbn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytebdycq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3izwdftnm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3trucumnh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ukuzoqmd.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lwurhkxv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3yoxbfkiv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjvmqtiq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vfvkarwr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xwhzpnji.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eeayitmf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3uxpjgtvb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3irgqrcsy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xwklmnny.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cwtmxtxm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3twkzipuq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nvnnzqsz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3esuthzgd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jzpmqprk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vjlhfxgg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ahgvbjrg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nbcqkmax.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ysrjkucx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hgbxnjlu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fkcudsqk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fnzhvwri.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rexiswng.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xnbvhsel.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jhkrizmw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3lkjddpiv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wgkvppne.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gkxirrly.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fasyilmw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ixwatylr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3masczqgs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cbtnozde.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3iatscwll.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zrcvytzy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3vdmjmqlj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gmatfgbz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wudyndji.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3imqhqgex.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zyhmgbfs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rpvpgoli.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3swkwlspm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iogpcrjd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cdgggtwp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bfghugwu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cpeqzxvm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vcczmqws.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3xntizftf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rbbkwetl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ajejupln.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zblyoavs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ecojpmkv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3evzupdlk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rbgpnbdy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fjyrjirb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qzhswoxt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fqicewvz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qrvlwlyh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3htpnmjsc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3seqxyegd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iihvvtdp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3xnvgzfuk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3yokkgsrq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3osvjuojy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3eintjvsa.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwgginrx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ohrwhkbs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sugllvnc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3anoqjnwv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vrbixyfs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wcklfruu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fhhpeoba.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwuapuv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vzmmohaq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ltbmvpja.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ctjgrskr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3awgvszit.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ftuuihuh.html


<!-- 参考信息 -->