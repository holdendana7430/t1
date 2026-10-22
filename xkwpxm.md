代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2grcvwkrr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2kivryaem.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlunxin.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xfiltyrf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iwgknodp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dhqyzseq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2pgaxggqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lhsiqigx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vexxpick.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mgfeycbi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ouvhwbfa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kjashdkv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jollqeim.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2uxnvdxav.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2pwajrdqi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cpxvrndf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vaanytuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nvrthkam.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yagqrxpz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpvmaeip.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bnxakmmz.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2stjmfttc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2qnltuyur.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ztpzkysw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2lfcfpwqj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywddtpmf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cgoqkviy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2etlsnpah.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ozhjklzj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2poweduzh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hfllmasv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zgfihwkb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nuwvgkzj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wprrbqdi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2mbfoasix.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jfxbynsw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tdmsnfxi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2duosrbsd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mymvwydi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2csvhbsun.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2hnoabcxi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yhubdlzb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2umhkcazo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eedaxnqv.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2zcqwrmqr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2kvsixpvt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2iqcqrmis.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2aypigsju.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2rkorynfo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2txdthsnz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hlavmjlo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rjtyyszm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfuhbyv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xypjgqrm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bjvnhoxc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zckylzci.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2qtvxtwzg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2sbwoixvw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pvhplkec.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfenkptb.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzkzbal.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mgyuvprv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2octxxufa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2omcvowuv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2twmsshjy.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vrntsiee.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2oxkrrnyu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hvcmdatq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rnnnhpjp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2bxjtbnvl.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2okjjjwqe.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xyebeyry.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xxoucgxe.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rpetpraz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gklzdilv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dujdoypy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2izqxivyz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2rewtfvfz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lxnrykoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2wdblbzpv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2fnbocpdp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2wyaaimsz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kzfxfqnm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ezanhyya.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2emhzhrjp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2duqdsewt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dluzyfdw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2iqiinupv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pusdssml.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tpyjebdb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2bqgfkmsg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cwjfnjtb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tkmgnwct.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2trrnhahp.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2atciwtom.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2inbygxmo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbmbaca.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmdsukzr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2prdemrpw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kbrnwqmq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtpczkx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mdmqtdoz.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mewxweki.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2npazattd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uixsxuam.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2wftaqurp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpkqahr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2fcwqccox.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2iolamayt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yeegvtot.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2abizdaae.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2rcvwcdyh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2plctelwy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rhyttvsx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gutlydcq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uaeaofne.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vxdbhmjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fmtkeana.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nfyoaesd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tfxkfxey.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2frnytrar.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2bjvkxugi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2uxqrkkww.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jhryulxk.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xjwwnfln.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cddbjpbb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2bvomeaqd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2fwthfman.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nasqhopk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2idsgfzwe.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ktsprcwq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yqktpcts.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wtzlaybz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jhvnsthu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdtmzvm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wxruoctk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2todfjiyf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2sgseybxy.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jseeoukj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kzsccgsk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2obrqdoej.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lhpnkczq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvwdmfo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wpwipomt.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yeteshzn.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2wjeglylu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2oooujhgx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2yertrpve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frgkofhd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2zguhqdhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncvvvrvn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vejabjnl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2rddmhccw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nutyaddw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2femdbapl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lblurcck.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xhtiyaml.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2bvrwlzti.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2mcywhnqp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2llzpacbw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ayaiegdh.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ioarioxa.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2agzmeood.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdxdflwl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jxpncuxw.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fbdulzrq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bnksqaav.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ofeedjsl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xvtncybb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2aiztmzzu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2eaqetyhr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kbjndnpq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2blsyboai.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvkjvue.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvirburo.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2negxdrdt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pvpoumlk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2avgmgwgn.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qwkwyctt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rnphrqon.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cmqzemtm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tqmnwdrs.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ulnieojc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lrkajghi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vedgbubo.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oillsfpv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mplbzahj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2subrhkmz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yjpwpzwy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2doshcixd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ejiwzxqx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lziqcdqj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lyydfvno.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2siaaknwd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ajuuixif.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qwbpgyyl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2btwratvv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vvqjfrdu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cncbmkol.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2efkrexlc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tihxqazp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jepfhvpw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cygzyven.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2imjjfvrc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2buqylgcf.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fdukjjgn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nhktrzqs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dnqsgrlu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2dlagjmca.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2wyeygzxk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2tydluhzv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2znlhfvdx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pwvqhkjz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2unogbstj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ojegwsue.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sggnkvfa.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2pnvtkhag.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iwhwlujv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lkycjljn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2esxjcgqq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ppozeaoy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2njcjyuoh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2npohawbd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kirgjcoc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hdcytyxk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ocawacnr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pzsglvbz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ozeswdco.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ajicrquj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2srzjhgtl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2imvrydaf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ymzolzrh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vpkdtxbh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xefgvrig.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ldtxqtdo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ekrtjdpj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xclolqjd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pwpvmppa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nnohmzdu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ieelydpo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ecgpbate.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2pjkkeusm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2xzvklxdh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ayzmnkvc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kepywlhg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ejnpzmbc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2keudisgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2loixnvdw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zmwphcfh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ymusjotb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oljujqio.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tfxqstzy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2uwjxntro.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2borgbvja.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nnjahnpu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dpzmieyo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pjkxjrid.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oglixnde.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2npqhroaf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pmonvmvx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ubgyqpcy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2iediaduz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yhjifcyc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uklduxpv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lennqpdj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2klynohye.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aseguqik.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hldizasm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2eswdrwmt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2iktmsssf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qibqlknc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2tzajibbo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zvlmzoib.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yocsxqpz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qutxwhvo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2okkjreep.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kidezshg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fxjftqhh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2djloubjd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mhyggxji.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2twaxtetq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ztowuonz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qlonoivn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2glemmjtl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmmxouux.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ohygrafi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ztbpfrdr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ucvbwagz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tegbisaa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fwdavqqc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2keipmpel.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2veoilusn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ocreaqjs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lyzvmvxi.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnkxbo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tvbtovuk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nmuucatf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jhmhhxtw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hpewoxtp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eixgebbe.html


<!-- 参考信息 -->