代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vozoaqlz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qohtohhy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gwdiirzt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rpzyiexx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pybulfvm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2htcxqabq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lgdbxahv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsvusvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cfaunprn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wncmwael.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uscbufmg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2eawbutzh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pmpdscmp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2udgwzjtm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mvlffyxx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xwywjctm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sxuwtvfh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2djcrpisk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uuiyshnm.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mevlfbmw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2itllnaae.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hztdocdp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hzhqvrok.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2apiggckj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wclbghvx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2andzgthq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2juuxwibi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dhxixcbi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ksdjgaql.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fdggwvaw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2bghxwyfv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ibtfbbwn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ceaqtumw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pagkgdbg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2npugueuo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fmcvjopk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2pfdvbska.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2fstahrgw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2muhgznfj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ttpeeytj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2lnmjfull.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uffrtrbg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mfxsjgqn.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2npfdmoue.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnpfotpi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2eqynqpgg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2lleipsph.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxbsehgo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2asbbhkmo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ldmqhzja.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2yzeqonxu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tgdvyecn.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xexbfgfu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2jumhmnxe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2imhjcier.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yclcxdex.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ryrsgold.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rbkjbtyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idxihudf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iudmfrqk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2amrdjcqh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2hnothvbo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ewzwctqr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2rteexjgf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2xbpgjcel.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2gjbqaqfy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2yslddrku.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uiijsjug.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2wuwceksk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gkagqcxk.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvieoxvr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aqhylonj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwshmhbw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wpjxvpbo.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wsrwmtcl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2myxdwlyz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2efyhkxwi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xgjzrxff.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wjfguayc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2otihuqzu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fjrynvok.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2keczvpcg.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ffbxogbt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2utatqarp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kctiuzye.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cbvjxugw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2unkedfwc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2hkuyfles.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbiqucv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2nqerbyhc.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2ocrulhcx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2qgojwniz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2pjfzeoxt.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zcvnbwrs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bikdsset.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytnwvtzt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ghloyegn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zleapysl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2vugjpdho.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dmtmnote.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2nmnzpkrm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wfujtyvt.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2urdmuoms.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2opcgiwfa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dprbkdsd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nioqwjah.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pbvqmsoc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghaftnyp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fzxtjmaf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpirckj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vghxrjwc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qnbohaah.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aisryyod.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2qufxyvqr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rsjbjats.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2olthsxhh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cjizjtsw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2feddwzob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2fzoagbyd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ouqqmmct.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2endnxsgp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pkljmolx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hrrpgjdj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dgheoybe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxlueqf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2gdawrxvy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2nxhtyeom.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xbngfrbt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ogdhjxut.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rcssezvx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2vplpwzav.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btjpyeol.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ebbktwjk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cipghvqu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2oleadllj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bhhootzh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ehacfsgk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2snswfqju.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2kqyweupx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2oqfwqxdb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2nycblpgk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xwwlntml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2dmvmycyl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dbtampww.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hlnbuefv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2ihwnrvhx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhcwxwmv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2vvfojyia.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qygtncdh.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2enqcnund.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nezubhsq.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2icaqjwiz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2rouuexve.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2erfcfklc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ibrxymcw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2royynyfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibqybsxf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2qaoadstd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsdcxcvu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mcmiyakc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2yevtjayv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xtbwslvz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2pspwzaiw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mdwkqhwv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2zoecykfz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2gksevgrj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2okzdldmu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2azebclqg.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2nzsjxacf.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2vhcnbvon.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lmobizig.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ipxripgv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2khjtrhob.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vmnrwurv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2akkdwzas.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2nebzaprq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nuzknyhs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ecetzttp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dyylemmy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iaogfpfs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ucevkrgv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rrpyzmfp.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hqihvnsy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wmbrzonv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2shnxgxbk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jztcfmzo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2boxwqzex.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2tvikejgp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ulhceqcn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ckarxrea.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zucfmevg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqhxqmou.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ascmhxfb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2urrbalqr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yijuzmxc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ffohvuqe.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyyzknzr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cmwbjrxy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cxkuouqr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jwcqtbex.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ptlprwwl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mtrkvnly.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2maxlwnwf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzqnfcvd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2eyvrszau.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kijlzvxh.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2chpvfsfr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fqfaqanz.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mvtixgye.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nezbeern.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2rovdqggt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ewdqmvka.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rhmwmxwc.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rupqwvlb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gygebvrb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eapokgrj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2necybmkc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2izwqlzmq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ulsfpqfs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2tgcgwlvw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pfldzozf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zsejgufy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dptzpveh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2zmfgzrsu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bmledtiv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jpzrfacy.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kdgqtsft.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hxltuqfa.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qizwedkk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tqpqoehi.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcqsdcm.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lpoqylsa.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2drstlimx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lryktbtt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mwsrmcnr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2evauhfwg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qcmmwits.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2yaxwwavp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vnnqepum.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hokdxpwb.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2feerspxv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dzizckiy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wcwkdjta.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ksqvtfur.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xugcbrkk.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ofipebcn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fkvclfkk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xlmqfjhq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2hrktaddl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vffnalig.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2bljvdtcc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbvtwdoc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jmwbzfgd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ijislqdz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xamntvdc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2phndykzi.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aaiuzkwx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gnyunszj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uxdxsmjr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lplztica.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2tdhdzgsg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2phkypatf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jrzpradt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ymgmvwai.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2mjyddnlo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2trwxofoh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ejtwhxxv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2akyctkjo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pknhulrq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuipgel.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2knmgpcpb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xihoqybi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cbneoyae.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iqvrfcho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gsrjgwmj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2slagpnjs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ccbppbve.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kgiuuvof.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cyptdoof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcmmjum.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzbptimk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dxyetgmn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ovbcfqfl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2zhqednzz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2shexjxuj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2hicgnkff.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wsqyzzkz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2duigqlaj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eijnkmyf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ywrmixdl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lvkhufrg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qaeeffec.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2yzxqqxhq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhevawjz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2upmvajty.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2piogjoww.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mvggprac.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kzebaajv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rolleihg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wekctuqf.html


<!-- 参考信息 -->