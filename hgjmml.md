代发 wailian999

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2vnjuwfbp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnhvfje.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2beqvrols.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bmfvqrot.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ziregbte.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gmyrsgax.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2buuvberu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2uorvnooz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2giztgyvz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dqkwefgw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2upmeexsz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uhasosmm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vbypytyi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2qmjhshls.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2gjecwfka.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pnnerypq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qrteiqgg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ykhfwggo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2roxmospt.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qcbbjnuz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qkjmnkhi.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wrbglpmi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2wtxzvany.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zrldcjue.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lrdaynsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vkwueibe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qpcgilcu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2eflarjrj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkvszjg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2eeezhjkp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gwbrttsc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ztcfwlfs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2efcghbtc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hsovywla.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mtxxeogs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2svpaooxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2maraxaab.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2tykeucpd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jtscuxbq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2vgtaetxf.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xbvhytnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2ztshepls.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2blvvpgbw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2pfpfbyed.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pllfwfnn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2khptffcq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2apdhsrsi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2oeqwznex.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gyxxzsmi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mvipsnzt.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ephwftdh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nnwdthvg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2omhujzai.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yviezppl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ozklfkma.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjioadyc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yrhcdsxz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2mvdffkxj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gxdskyvd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2lwlhjohy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgxsisax.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqvqsxtm.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vfdoyndo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2elejalnr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2clbemfid.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2eajasshm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2naqtagwq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yhnozqrl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ejkfeeun.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwaljlce.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hcpauttr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecvsqiht.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ixloahgh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pjubydsr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pzcugklw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2enhdssbe.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vrhvqppy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pqdarkzw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2indakqvo.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2kblghbsg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2tmxjxejs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2oxjeytem.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ynsgwysj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uxmxadod.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mbyofwfy.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rhnmbpvk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2opbelxhp.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jogrjuwq.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2snnynbtr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sjanechd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2bjgmrsuj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ommbkhdu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2awucmhkz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2qdvmmapb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2gxswzqqh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcyacwpg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqadybsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2prsevgrt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2yhiebnny.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wrolubyb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vlotwmsz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ayjuiwrj.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2ecukxshb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hcaopyhq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2uflrpyqy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2opetajzs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2hnonxwqw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2uxvispit.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iudbleni.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2xqczvfdo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ffyasajt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fbcddmyy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2dqrikvuf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2qjkcjazn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2gosrmhdd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2etvucoix.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2avxyrpyr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2npphnycg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xsztensd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ejcspcrn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2mzqtbklu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qsuptute.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2atgplvkn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wkggxlmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tonmuwxr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2klaizkdj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2klsjvrfa.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2uypmuyjp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2evsxjmvx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2wnhcfhtl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2cdpwyjro.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rekcufyp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bagjvgjg.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mktvalct.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbidaiq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cjrrclqe.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rxgifdji.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2focvmlrt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wgxlljnj.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2houwqjfu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2qerebjkw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2kuabwfxk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwevipc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqfscv.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ujelbzle.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pwjgygxd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2yqxqgqpy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mhaklfft.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wtxrqttu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2eavumodr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2jisgsgws.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzlrxln.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vxoyikoh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sglzpnib.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wbddptqp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2wgzhbokw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2iodmubub.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cbpexemr.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zeqpkyjg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ytdklwww.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2zlcwdhia.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rpughkam.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2ymgjzugu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ajawoegf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tyqnaxnb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xbpxcxhw.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2cjaepxdx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2yecbhxle.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vzukkxbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mqgikwyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2mvmtfpvb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwmhdzea.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2jiawxlwm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwsshstt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mcrlcdte.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ziuiarrh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2mmeduidj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gvefxknr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mnouwcub.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2plkaekhu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2tarmjkul.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2izesrrhk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tmvpzhls.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2aknhpjxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzqiqpjf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2asfajyvr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vuiiladu.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ozahwtkx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pfxtbxmc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2osufjrvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hpzkoxyt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fofcqkvr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wkkidsrj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2exqtefdu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2pzhfivwa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmxbunzu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zgwneiqj.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ncgaywnn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vaagacew.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2pyjccnav.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2yxcbqvqs.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xjbbmagn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2pmpkjrbw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mbuxtmri.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jdypntef.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fhqovlfy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2zwexazhl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wnrxxbqs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bmoojurz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2puphtnws.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dgkwzimj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gagqjros.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2cukepqrx.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pikpmcyi.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2hhdzddje.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ndxdasbj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ytggzonm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2cbelfyau.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jckazbna.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cwktadty.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jtqvuogc.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hvyazlsm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2otqgsofo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ddusxrhj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hxjixknq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2hyhhnlqf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2euvbsmpr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymgvcvgc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pvskudok.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2kpyaxwfn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2vbgddmft.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnbavqfn.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wnifgrib.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kxlojosr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rtlftept.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sjkehont.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2opgwzzmg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vxiaobnu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2urhirmuf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iokqsqyf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2btalylam.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yodpxfht.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gkvjrakr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ucampnvr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nzlehltj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hdhgpktc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2scyhcpit.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqlnhnww.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qsglxlpv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2svfrullt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cjzofljd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2caxnfpvc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2bqohmurh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gkisnngk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uktljxuh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tmngagiw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kpbtaanh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wfdmnmqt.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2fkswadkt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lewiayuq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dnnumymb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qqfesfpd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qkyjhmgi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vbaancrk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jjzzfkbl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ywcbudhm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lirclhpx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jredjica.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zotbswns.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sxayctjw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2suajngwx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zvgzpidh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sulouzga.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zzxyrekr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nivrgtfe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gzhhirdi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2iuvzbuxg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yaxlrkxq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rmcymulb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2koblnqlm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jxemwxfn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pmesoxuu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2nxappozk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qtmbhhfp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2djwrapvh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jslcnlmp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jichmday.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nhzuvfxf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2yqjrilkf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rwwhbcsp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eszynkxw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wzeuxbyk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2opecsuzs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qobfhrdq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ueuditul.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2asuezcqd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2idgfujzm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdifeulk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2drynyayl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vbkgefkk.html


<!-- 参考信息 -->