代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfnnbdrl.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2akeemzvm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wwdlfuvc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zctiuzqr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qzsvlmji.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aonktxkp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2odavcqmz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pmsjvody.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jhctblpv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yaaxgdpu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ezgbnqfw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nvujpsow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fpqyezwi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xulvgtaq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cagumkrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ljxpbhfe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2discjysz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2palidpue.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ldlqbsju.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kyrgepof.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nteeddlx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2trtrccoy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2cqixwzze.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pzudhqsk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2eddrthtw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2sdorpksj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wczboily.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dxnucubw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ftvsdusr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2gejqjarg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wxgamjnm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2gnviocpe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2pmrohyhx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhvzmllq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2txxmzyzx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qvmskppc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wfyhgcha.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2epuxuqlb.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2kvyoorzt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wlnkipst.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wktlfklh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2lotluauu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2otvbdoth.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zswglyay.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2nrrkvkam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2gdfovlfb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdosfdgd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hmhmqmqe.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2edglidyv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2llstzbyr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqwogwrx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xddjfcte.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwqxhhtm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ferwuchr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ffpdfsjv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2agmdhubt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ioiypvug.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2cudunpfy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hkkgyjdl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2cgcrrica.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2bqpuweez.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2feixlkjv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2crsrkiha.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qzrfogye.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2iqgyfgtw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zpwpbxva.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fkcaoojn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ovcxsorp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ourpzwtf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jmxhtjxs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2gkqfscyx.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2slndnxnd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2zdqapswg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2makmggzq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2dhhgtsuo.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgcapkso.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2twmrsnlw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2baoosqzq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2odcgyqic.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bcggatal.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfwfjcho.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2znqygzeg.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lictfsim.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2fcvgjwet.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2osahhbet.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2uvdyqzce.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2srkawumj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2othgrhlu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2kzkntknd.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2xfkisatq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rfmsmfej.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xajqgtzk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2mhrtrxsv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2faufurdk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2hkecpejn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ijunutlq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2giexdgev.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fzzspubs.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ncofpsog.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2xkddapnj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2nhhbitcx.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kdkmletm.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ryzmujvq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yyxperiv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uvtxzqnm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vgbfcsvm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2excoopiw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2zveqtooe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bxdomztl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2fhrzcqfc.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2arzmeyod.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qfhscmas.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lohydaqz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfszlwn.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kdzpskgk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pkoozwdw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ntsssqdh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjxfhnp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pogxoezq.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cjrfgmfp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztuxxfeb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vcbcxqzv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofyiwbrq.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2tjlxdndt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ecdqymfu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mkdhanbq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2agrgiing.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhcnyuo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2evrbewwe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2ugaomlvw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ktpwgzge.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhzkkvub.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yvkjpgxg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqatrzp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcdokkid.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jybrmqmu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vuvtqzce.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nsdwrjei.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cnkwzzje.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ffsxltsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xmtrkpbg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vclyjlqy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2egmtfxdj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2nasqirbo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2cumdtrdf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2ogrzimso.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ivlidqfs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2uywstwmv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xofswvxa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aymgcupw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2lpksugvt.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwuzdqxi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2uoqryoyb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2kkqpasin.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nkzxxwfw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rkhiwvwo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2agvmfclh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mqjjpbue.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xlhldczk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pakgrsld.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2fzisuyyd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dsyxlfis.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2zafqjhgw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2scutggtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2smxjtpbt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2grsugbva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uhqfszya.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2behsuztp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2lucebxqy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2uhctjfaz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2swctyvte.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nhfdhydr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2voxrwcet.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sahpnime.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bwgzomrw.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kmtdypuv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hrinkyzo.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2koqtabrh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2mfbjfsgu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttqquyef.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qijzbalo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dvddfdkn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cqffkoqo.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kirnfvfs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2owykwjvj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yfjufkol.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2zfcfjsly.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2isbsbnwt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2abiwzxxn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2waipidwj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2txnqhnve.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xxjmpzom.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dfkwfoaz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ncgbumje.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2woplgyis.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qojsefen.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wggymalz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2kvfwwxac.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2chpvblqu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2etdiueec.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bsonavmf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ekzhjpvg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qlajnohw.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2rmfraedb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozzghiff.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ucdihowx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2agctriyy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yyufctbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vgkatzug.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmtdsgy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2atjjoxnt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkeitdbs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2fgoqvbng.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vjojhwos.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmnyovzp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rxgyqxwz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aaqqtnyt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jgcsinne.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ewmfwoyb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ohvcczon.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hdpfxdgg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nbiqthub.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nduahheo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ustprkww.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nvisobvx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2thmflgst.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wntjzqif.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2pkgdtdjl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ohparqva.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qjftwvhf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kvlakxyx.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hiphtgee.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hvolnqxy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nmchjskk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sfvheguu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pwozefxz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ehpywcoc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2enirwqxp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2opfvoslm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2nwjlphil.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2phiqakxq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xojqjpzr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zhgivuga.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lhatchdh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rdrshutl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xzdgwmph.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ipvpucfw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cuvrvdjs.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ffbveccf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bdacctqn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2vmtoiunb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jyntblci.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iwyoebuk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oiotzfvz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ehnazlke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2klerggbq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2epuwyoee.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uuttjjmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wdptbjtg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mdpsntdj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ukarriey.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rzhabsvl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2skeraaia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yrjybtbp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2imhobkkf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yadmprfo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fquxkfde.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mzmeytcd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dnclxaen.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mwroitqt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkzwmann.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mzamaasd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zshetdqs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rholvdsh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ncpopbzt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gahmtclg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hdystkxv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbfzevek.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqwfsbau.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yixktgbx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2grcfesiq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2giswlnuo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mzmudrwp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cmuvxjil.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gpdgzmxx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2qqrdlqlo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cqijdfoy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pygrqyfl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ipfaelgb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2joxhwmrb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2trzpxfyn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lygynczx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2goencpuf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zjnpioqr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vrqakosk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2osjopaks.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zdlywcme.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mcskmhqa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ajclpnzt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vwdqfhlb.html


<!-- 参考信息 -->