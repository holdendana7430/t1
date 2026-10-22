代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ixiyhmux.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gnnfwbav.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2qnoofcoj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2esrklfyp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qtcadgso.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gxunwebv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2oehpdeje.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yspxxrdi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2uzeipbse.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xekzhrce.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2arrzfiix.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qpiuvyvt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2wwtyudto.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fpwdymoo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mjoqdijv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ywveicel.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2auqlexma.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2thftucdg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kmaktdli.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xsgjtkgw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bhssodyv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2llmtudny.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2cxouljxw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ahyadhyv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2zkifvpcr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vrramhja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2midloknq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2youndqfr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2hebfscph.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vamuiuzg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmdewm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2helyziah.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2byqjdfhd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oayxuuaj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vsshsxfy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2foghraly.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sguencbf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wrerazls.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2icffucmx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xgyxchva.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hbpcarel.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2glknmxyd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hobqdqxo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2qvesgteg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2alryyisw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yqyscwqh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2tvpklbjl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nszgxkla.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2twjmiwyo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bmytiszd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ohjagrrs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2cklgrdyu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zxtmybsa.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ktclopgg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fgjpclea.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2heksyxeu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2arlumafu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xohqhqfs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pyeyuhwv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2kyzvnkcq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nrrqlbzg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpytsrdy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vxqohxku.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xgbmvkhe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2jsougnug.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2guxsguae.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2boqwpvsy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xypukxvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2ukzxtpyq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2xihbpamd.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2httnfjjs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ymazrhxc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ratgdvtu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2psgxblvq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uewbbtki.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jrzjmiut.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2fskmmept.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2vbaaoncm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ecnpfdbg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkzqipin.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2svlfghpq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qhukurex.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mvbnvrsb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2nqarqagj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nuhnszqr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nzrqpulu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vefjxzew.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eqdxvaxc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iiltnpuf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bewmsgzd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yizkfdov.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hogaqdut.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vtwvmlpk.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gibapmak.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2ruyxucxy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2swabvqkv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2xthfphcm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2mdicoiqd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2aeyhlxnj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2avstqhqz.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2yrigggen.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jpaxxdew.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2ippnhtsv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tnkxjjih.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ojdbuyxx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pncpovze.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2erbakrxv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2yblbhywn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2djtnzuqx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2skvkfmtc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kvxwfprf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2evhuping.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hsydupfg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2pnoydxpp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruozixoq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lfccdxae.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2zsyrihwz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2wjdatsbp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2inzkvrcw.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxfvgv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ugjleopz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dorplaad.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hfontabz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2sxpokmbz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ryrjqwnx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jwdhcqtq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tufzduyh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjxjnnfd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdkspxfu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfhcffpb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ldihvunp.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2oietfnad.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2drhmylxp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2klhdeoho.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qwwllmvs.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2kntwnazm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ngzkmrak.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2ufbfuprd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sdrvjeoa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2tsszcqzo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ftbkthvf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2fgrbspwq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lbeymzru.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tixryoca.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qahxoaii.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2wdmohmev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2teiiqodc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wovudkzm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2cojmmndp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vwuerbbs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kdsojpxs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ccwvagdq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zcflovgr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zjpfcuer.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2izofyxus.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2jxaqgjht.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yauoairk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2imlgxlqh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2uavxeuze.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2rhrfyild.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jylmmefp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ptshhjdi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2woojqify.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qqrtddfw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2cqvsshik.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lgdoncmo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yieopfdy.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lbdmocpr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zwyngaqv.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2axodloal.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2iywlqwyr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kdyptueo.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rbmcqmuh.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zbtagwvh.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2voylshqo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cgymgffr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmomtgeb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2wcmmptya.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mldagxgz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfjynrhq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2qdumbgtg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qumoupql.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fulyumar.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2asibljhw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nbjvorqw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2blxpxdjk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mvpnasjx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ogiegaip.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jglahayr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2bdtlqdcw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtaijmea.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2njqglcta.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iidxxhyl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcngefdc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqvxqhe.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2axucloil.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ferkatrs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uvdtfijp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mggervkc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ymplhlnz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rnmtdzzo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfsunax.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kyzgcvhd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jsbndqyk.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2wbgdhgcq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2arlkqwdg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2qxogiokh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2rqltlrsq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pzsatrjq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfsuigt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wsfzwvxm.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jzhobbki.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sjozqcog.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kdfrzxga.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rhyncrpm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2fiwnozzn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sibpyqlp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dnivieml.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hhonmrtw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jxbopxpv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lcfzyhxy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2dweyjmfy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gruhrvup.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vlbrpapc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2yxyumxor.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2yesczodl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhopho.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gisexhtf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wppgairr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttojkmrw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qaobxdem.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ybdqllmy.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mwvusavd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lckhdkao.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rvqxepje.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2seqxhbbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmpibvm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wwqhltsc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2jejwncpu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2smgloytf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xmtqyyty.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2oyatwvdu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2cppegjwm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2daiwmhnn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rtytcsct.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2suadtfwb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lvfxwjox.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rghfcpfs.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2skzaltuf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xclideig.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2prfmnfmu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2undumpgs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2cyteuvug.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pazbrvmb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2idtfqdrj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rocpazrd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2oenlatcm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xhvkycry.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lrandtiu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jiitdesi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2yygqqsgs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gdooltku.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2navvbnqi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cudlijun.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iwcodzss.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gdddprbq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wopnagsu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlubade.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2zkwyorly.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kjremrzl.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uryoszsh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rspvqwzg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lgzhvejt.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zhmwrfwg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iopbfcfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ouruityz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hgjvuzol.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hvcmlkqd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pnblykkz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kjnsxpcf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bsmqtcws.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iytictxf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eyaewjfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sqnczerx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2sbdlcadb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bxbvpgtl.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2wsuwbgpi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hipdbqgu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hruqeaio.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmkfrbti.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vgtukumy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewnhjvnd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mxtcoehe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xhjpzrbs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2quvohzjj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xkwhvmfo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ntfejyew.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bsgbaoxo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fjwglppj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xlxzyeao.html


<!-- 参考信息 -->