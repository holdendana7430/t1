代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pltaoppi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tyxyljpy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kuqcmduv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xziivvmz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ldrqcnlu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2egrkuktt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hdonvxoe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2rukaypwt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2slhjazim.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2qnhmlneq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ghezuhhk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ndfjeupp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2lzyqsbdm.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vyhnkgqk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ewaldigy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2tfojbdxk.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ikvdumby.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2udqvscyr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2oavdscdb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yykeuuvj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2usmwarhn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ijarfuza.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2orcwrbjg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yrvnrhie.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atqskqbo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2wepdbeap.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2jpnpzmwp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2aslufgfu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwuwbssx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sxmfeqar.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2sjdprkvd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jfztuhno.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2iiccwupp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2navctskj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wvvstoar.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2orkkrran.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hohpodug.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfmveiln.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dybpbrbm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2revayyvg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2srnjtaxy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2eyokihjg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wrbpltsg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jztovtzc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2npbxoayi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2yakgbrrc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2qejiscub.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xpnayenq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oatmqity.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2grixnfkg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2tsbcqktf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2xivgwonx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwtfgdmc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2sfjxjmiz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rmnagxeq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kummbtsv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rzkvnhvq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wfarbjac.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zbxylzto.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2yklpjptg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vkaoafaa.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rqvcounq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2uopxselr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2plvxvzgh.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ywawqcil.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2iulchdpw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2rqbvkyen.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jyuggmgs.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2epcodcne.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wnoockko.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2qktqfjvq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2ebmwrbcx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2ipkfmbvl.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2oxjmrxst.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hxavvcqb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2aduvavmo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uzmgxuop.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2mcptwyiy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2yzptujng.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eoizjyww.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tsztndpj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuptwpuy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2vbkzrcvb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2wzyvhakj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yscerecp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2rxbuebnq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fbejmzoo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2utlyksgc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2upgohihi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kwnmfufr.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2fmgasyfp.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jpxtpikj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vfidgorx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tvfwjkbi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2uorcuwep.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hzoryptq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mgofomxr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rzzrawgj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2yltzfpch.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pqxxltzb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2bhmkmprq.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iipxkrys.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ywkwtyfm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2phghkefg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ittvujdw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2molbpref.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zaibjxwy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vwlcujrj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhkjvyde.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kucfhijm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lggbtwcj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2lmleadus.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2vzjuwwyo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bfvjhacp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cfdtcfut.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2dhctacir.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2npjwibbb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2smfgjbkk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2lqpzrfmv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jomohjtk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqekvfw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2njcauexi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kzvsqewm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wdseirtt.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2xdepxylo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2vckxloau.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2utpndrvu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2bntpwhgw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubiofucm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wrbhcmmq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2fbildvbu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2etclijoc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ejiosgmr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2itrqckbe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2xbfuauac.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ndnmtyqe.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2siffwflr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2vkntnnzr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2yiqnwogs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cbizples.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2copfqtgq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2qujgarqb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixexfgmo.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vteplwfy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2tdxbkxqn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gamwmttt.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hgsgzsxs.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jbnojwqa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aicmuvmc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2dhvnnnxv.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2drbtoslh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hjzcdfci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsxkrpmv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2jdigukej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2atvweeme.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wlmgcdyw.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2izdjenul.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zqpyggat.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dnbatqeb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2suyiboiw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ludsginy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2yhmuuior.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2etumebxo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hhelvdbf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2uxkgsvsa.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aazoctzo.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2diwbpgvw.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zcmembru.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ibikaoup.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2erxalfdt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sraanbiv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mhpegdkq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ironhxxu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2myaugfng.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2bzlqkpmp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oasshvnq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ykjowvjy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qtlxnluf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwjqmzf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rgqoyurx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tzocwexm.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2zxewqrzi.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dbawdkfd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wexqghae.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rcqnyfau.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nabywmqo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ljgtnfzd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2kwouqawb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sictwjbo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eegoqqlz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jdqvswwk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bfqtaniz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jqhrhfpg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2taglabmn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zqtvbkux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fwjurmxd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zriojjzj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2oalbgbtd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eldxojqf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pmcqceyi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mswtteyu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dbddluhw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ullbemxo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jpbhmwqo.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2leriennf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mjbevfjr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qczclqbs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjcgfch.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jsahydkl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2conrzpgo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qywifhmn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2odnxdkvf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2otwstbho.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ybazvzro.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jambxdpq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcxaiso.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fyfapkuo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lcirrqai.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dpljspcv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2mduxbnfy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ovxxwxbn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hemgxqbu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdyrlywi.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2bmidlron.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2kjkyimvo.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ctelwscg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uwysgnvi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lpvwyefi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2czannlfr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mtwevver.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vsryrrff.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhkmltq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wzgnnqdr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2qknttpxz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pqejbwdy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xzbhbafl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qbfikwmj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hnksbvum.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gehidfzg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nkdsiltg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2alrsavvp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aedgwhuk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dkvuspvg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nqidbqrq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2avjjyvyf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2laedqrvb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wlvkysia.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwbhzdvs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eidzbixs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2abzukcvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ipzxzlat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xdoyiwss.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ueqypzri.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yjaykdfh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zndfzfmf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sejvdxzw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pqnqbqbj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2narkzbim.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ulfseqmw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2bcgagkvg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2teyqykkh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eqsdmxyj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bdgerjom.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rhaiigll.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2admhfsbt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckphpwpv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhcdzogj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yjutrzoe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gpmkobsf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2tsorscon.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mlbopnll.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2myhvrqma.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2edewqnmx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xqgxcigt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2phnxmeuo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vbasdqvu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zomcjftx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2iniydflf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2esmqqjrf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fsjqqmji.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfambuz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bhuwapgd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ymmyxjkd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bnvukxvo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pjswovxu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pvgwzlbd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cuxzelyq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wfskscug.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2wqmsugkd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2otupiykd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ugzunouu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rfibebdv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qjoidhxz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2igkztfiw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zdrvxvbc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ikypkrym.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hkmjulmi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2atgngkri.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zshlhxig.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2nvshsaay.html


<!-- 参考信息 -->