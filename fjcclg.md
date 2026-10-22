代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mitaxbwe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ejjljwfu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xlelwfvb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2byminxkx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qdirxqwp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wfppybdb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2odusppvg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mkwxcqxd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2arkcudwa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pjmvchxv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2rwoqymel.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2abgwtrqt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dkkgchco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qambbmke.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gbiphkmt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ieczaoys.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pmtzekzy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xvfzdwlo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qlcfzeyf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qgspbshe.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jqhtkdoz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wzqvkzss.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wzxvuphz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2cspyonkt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2quzkurat.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2cvemibqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2qdswcdwr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wrzniddf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2sagrhsrg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tycusung.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2iqtymkkt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2goplqdja.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bmeacwaz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2bbalpini.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2xujuaqkd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2nzpilztx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2yjyyhcmg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tqblzogw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lkjprahm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2hiyqmvuw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ewlrkyjj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2adffcpxb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zinzquyv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nopdcdli.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nmizovjg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tjslyvxj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2xjnjkozy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2oyuedhfp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tuvinxtl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqnemwp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwktwetx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2oaiwmjsa.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kxwsxpei.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xskwowwx.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pzlbsioi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2eixnvtwe.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2sbhncxxn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ratretmu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wpjwybvc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2vcdyvybk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rwfowkvf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hizrgmlw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2kuqmdbvx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xlsvaiim.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewzfnxli.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2efnbjonz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dpfyydwp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2odamdnrp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dqxjijvs.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uhiquekq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kzrdzhxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hizgsbgr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ulqjjyvm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mmgsxqkg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2awisinxf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iasyotsj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2foeahnbi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oyrmtlnr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbqgdfs.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qqzrpfuh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kpbycmaz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ukxvngyu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pvevpoii.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2lhulblnh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xrovfsxo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2uevaduad.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bhygqspa.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iihyepbo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nbtbuhwz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2jgdynyzv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bkwdsrbq.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hkdxvqtq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2tdqauldt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2zsdrqsuo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iecbzkdz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gyjatruz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wgjsszyw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxaqqpip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xerpwaat.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2giuadhek.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2biboemsg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xqnmouhb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2udvtohkh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2knklvkcy.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rqpndhtx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hkryghlz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qakpemnp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2kxmosxxn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2kdtzamek.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2headtqbv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2sivgczmn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2jpfukmwh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rucjfhzt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2szxnfgzw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2eshibhlq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uusgfega.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wwkjenus.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2gbwfbvjx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rvqtbdqj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2utvuuhxe.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2tgadxfjb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2saujrpuk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2anibyjaw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kyscduii.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gonxenuh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ztogvlnl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xpvsnnpn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2phbqouis.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qyuyirup.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mgiaqnum.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2potunadm.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2loxmwbeg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vgzbsmti.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2iyjkkotm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2naszlqcu.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vffhyedp.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2cwsaooqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2utrerdex.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2zgwnwdkn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2myowssug.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xkqohpij.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wayanpaz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cmptvszl.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpclpnww.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2grejjevn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uoitwkxk.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2otjwefrx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2iriuvldi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vixplkmw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xlguqkhi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehbccqmw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2xwjalqvs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qulraegp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2djkhvmjy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2msypdsbx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jhdacohw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2eifrxttm.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zxaojyyc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2teiabppl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2usqpduhh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2gtnarauh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqwdkkp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kgxfdwnm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zfomkwgh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gdzsycso.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2tsubsmdn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mijpwhbm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jansngvs.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2oxojtnfi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ukrvglfn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2claeeppp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2xcfzxqub.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2rgpzjakd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yrxvaczs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wbouhkxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2cdbipmhv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2epakellb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2ixivcywd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2efokbzzn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ocxpimuh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2mkfcautk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2eyjwsqwe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pxrmlnry.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2rlqaiyot.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oaysfjgp.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xpxrrmbp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aaazuxna.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ffyamfwa.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2jefuwdan.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jvxmcbeq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqoegz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wuwkxpby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmriqone.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2flojfzrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdeofcsq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2dgqpafkb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ovfwluyx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fushohoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2inbhkydt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rduihwqv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2eyafixws.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2nyelloyu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lqxccbpa.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dgjkloto.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vdvlzyiv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pwmkhscn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2geggaths.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqidjpw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2psaqfodv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2czugzpmk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ckmhpsjj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2cppnusdd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2hazagcop.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fqhtcvqp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lokohjzi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iqctdapn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2brfbfaiy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cjhasxle.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qrextfia.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vsniogwm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gwfnqkyp.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2qbmohaxp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2khokmozk.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yleoejnr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2tfgcybwo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ykdvcede.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bvmxpmsb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aphoxqtn.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2prrzpmng.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ogcfhtiw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ayvzvdho.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uyfxmqai.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2crwwsdum.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2aqxnlndj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cznusmnc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2fwpltckv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ogegisjh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2mbhwisyq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ctirsyrx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lymsnanf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2hadljqxk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zuabhpcp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vexxxpuf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnprigv.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2islpsuhb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2huwfqpas.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hgrbbein.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ausrtdpe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qcsfnzbr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2hpekgsnm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zvfipcry.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbfyhrjv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vtbmftfk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vjqbvzuu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2saxbiyqz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ezbrqakh.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2njyfqxbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mzozrxdr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2kggsjqba.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ozlzatun.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mffvfdta.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fxynfkuq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nwzwbkll.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vlxlkoeq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2cktotqea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vyxeldfv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jevwgyzj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2zcppyegh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ryijiczu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2rgvjddiq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wrwznlev.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2bnmajhlw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qgobkdpo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2xtcdazua.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xxtomfqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lgqajeyg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2sbunhuqd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2boqceass.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2byqhsfzb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2otlyqfxa.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pwnzhcri.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hymzvail.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2biirmhjs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fujjwegg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2grqizbbp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zwmxqxyv.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ubmuwlix.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ouabhocf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2crsnizeg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2msfhknbd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mowbqhvr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2clkhuyhz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tnaxcqgt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ddpciaqe.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wstulimt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2udhftqad.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wacbpomp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aquonvoz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vzkmhulc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xbrlbsxs.html


<!-- 参考信息 -->