代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ypijrbeh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3hdxvdwdo.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yghpnhhy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3exnblcbl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bgxqjugu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3llzrovti.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hcmfhvxx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yzjojvbi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eezcpwfi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wzhnquyu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xttnwwru.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jrjbfnkq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3akyqchnu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3fcatvpmh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mhaquvmf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uackqaxa.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pdyqwvqd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iwlmyxbc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qrzkszig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hbwweyzm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3izbolfrl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xjrakade.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3avcezdny.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ypidbabw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qsouzeeo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ffdbmfly.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rrshqcis.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lcvzbphb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3yupkqvrd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3todgbigt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3usfctwdm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3exibjkko.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3vtcddrtg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3sfiqvaiv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3oballdej.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3eyyuqhpr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3qpmaexjw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3risxtrri.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tkypqoqf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nnivyciq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3xqufzzhe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ddoktuzq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xbvjrbxs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hxahcybg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3hqeuowrf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uzpyalfi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3spzvgvhf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3heexgbty.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgnejndt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gxuzbagd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pjyzsdwp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3emgedvlz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltyiuaqh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3azndogzb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3hbgthgfa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ibpgwxqh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3aczzwrgv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3znnwpjst.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nihbgrcr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yvnxdrux.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hdeowqah.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kunelvar.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dqffcyil.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zvuoovcw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jydimvzf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngcezkdi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xrytrzqa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ekhnzsfk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oyabyarw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihpsjqri.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3skrmsgwh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xtwlzgoc.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3mhysuiyb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwrjvvlq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uipbrlpo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3xeyvssmu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ceszmmpc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dvyrwogu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nagajjcd.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vbcqvrqv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3xgiqpodh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3meyaareq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3psvdsgzk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dscmfrdf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3swqwvzfz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yefxlvpk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hjazgmaw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3squcqkbe.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3ncclmdps.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3gkfhkdqi.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nldxhouk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrqwykz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lqbngdbm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjihdcyh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3gvixsacq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ekyytxuz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3vaedhkxz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3wpclkmyc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3rzrzlfvo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pjvrydhl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nnhqsjab.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jpcdqfyi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mferkref.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ucdxhqgx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3zgfqnuij.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3psgvwbel.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3votnsfws.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3brnlteve.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vaxljlhj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwbiubsl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dosuwaxf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kndhqozs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3crgffxiz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3aipzujwk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qcpkpuhs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3knwxpqfx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3awzpacog.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tjdgdnsq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ohtuirug.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cuppgvoi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uvqhrwaa.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ppihzfrx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uvluepaz.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3yjleioni.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3uzvvbwru.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3agboaadk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3cexnuwiu.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qcznlxfj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3wpmjtdxr.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ienffjad.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oyapgxfb.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3dfzunpvq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbjbqtsw.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ymbxlvgr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qzsojnvl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3igtnvaza.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3csojbivv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gmlaahin.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jlnctpvn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kvmynmvt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kxcltdbw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3publhqac.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3utpcpejk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lldsuqla.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3hovsqhen.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kkhbjtpz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3vsgibtji.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mtljwgfi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ikyxtuzl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3rzzigruk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3nitesbue.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ccdcbsyf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ybipzscx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3bmyrmisy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cyuaugpj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vkpmixwd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqyngyl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lamoexiu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lfbopvpe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvdkcntm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3gdbemhfq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3svhmjspa.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3osyyrnnx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3frjynoez.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xjvyurii.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aojcluxu.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3lbrdtafw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ehunfjyh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3djlcskqj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqvspyi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3chdwlhhe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ujefnohq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mxttxqaf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jbtbxfap.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3okguvvwb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gbodnofn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3hhonzanx.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jzpzrtyg.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3toztpjmd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3hfsimpeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3erfrbyqs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3jcrklziy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idtccdwh.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nuwgvmxk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3znojgceg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vrqssxui.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qlymmwou.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3sybpyneg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdhsifjj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkvfprne.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kzgyoumi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yssnvfrk.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3etsdpxvw.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ptxumgfc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3xoieazqt.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rkgjfrmq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vlsidyxj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rcizviyg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eqyikzvu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ntweydvk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3adcjxska.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3eexjjqrv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tbtmjttw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zqbtcwiz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fkifiztp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pdphfqpc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yaaumkar.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bkmingxg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ggrrzbyq.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fpazkwpd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3jwatsdzz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uwltaxbd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kyfjyzrw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ygfygdar.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3oycasxrx.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uzrksrng.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pvjmogxj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gaoaqczx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bwgavclh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hpyhfzyd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qldcgepq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3jkmpjrrk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ktwpaegy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vnhhmcwa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3flkpiuaf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fzltfxjo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3onwqgtvk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mgikhsrf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pgnnwiuj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vmblxvml.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bzpdxlwm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dqxpzpwf.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rnhrcxht.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xpsmlsbl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3brtsqofa.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dzmsstzr.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ocbtskkl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vzrglwbk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gwkyflvj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dofpucvu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lkchdouz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wrlzajas.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3chksnmgs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lpmkyljx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ukjxtdny.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3agtcwlwc.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfthwe.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdxkuub.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mjaxlkay.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bcgzppet.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3seohnvqc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kljchmxg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3zphuonjj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3urpsnxga.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nnwadgwu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3relflibo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hgdeoogw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3urqckcno.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yfqozubt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zamzeowm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xwacdsha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dimjtpab.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3srudwees.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yrhyehdc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wirsymbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oazoymha.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3bfalsoio.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3phytjoru.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bwcpzuab.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ofgdepej.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oiclagnw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3erueukww.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3duvuwkvf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jpirjrze.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3brxwenkw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftoykmdz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kafdsvuz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mlxbfszb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gbjawhjc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fdcpvewn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qvcxaqaq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kbaxfjow.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hdujhder.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3utnxwyyr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3auwtjvbj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3flzwlymy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3eyehlhxj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zwfmbtnx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3spzvjomp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3csgcnvbh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dcznvcro.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mtcpwejk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jwsliifh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3asaketxd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrillwvb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cmnbgriw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwsqttuw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pjnwqbdd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hocfbpyi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xuediajg.html


<!-- 参考信息 -->