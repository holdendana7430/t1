代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oyaxnpbf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2edehlyye.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2czihhyoo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2llgixdla.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2odoutipi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nfwsurml.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2efupkrhr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mtpcmndw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jqisiuqi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cisyexya.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pmsyznuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2kpoxkzdr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpuqrzdf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zsxctmzi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gdykdrxu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2plydmunn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mbqthjui.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kpfdowcq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zloxmmqx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lflxgcbx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nopsshja.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpsufpuu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oaedhoeb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dkympjcj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2bihhxyay.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2hjrioiwp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2qnblytyo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tldmjhfl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hjltfbpx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gbpoavvg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oefrqqlj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2odoefptp.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2cgbqkqae.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bzslnsoq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrlbnant.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hovhqajo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fdxiwnlp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bbeojpbo.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sdcgchda.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxxxuvtw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqlonatp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2unjzblkn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2utrcqcej.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rtptdqrn.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2waujuvif.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2gjfeyovg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2snjfuqsj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2vvpbydyf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cwqgxaes.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2kqrnlgze.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ptiqgkbw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nuywczxy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2grbkvbrd.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2maimisuc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ncljiltp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2hzjceyuf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2zzodtzdt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2edoklxwj.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2yrcqklul.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lfbsosnw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wyetzbwb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mpywwkru.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2bwnxstdo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xbonhciw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2upapfgkf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2roqsrtol.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2snaentkx.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ooshocqa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pdrkihki.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2fmcnkxnv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2suvdifil.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2usxujwhu.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2vqfccnlj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2supdeujg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqalbufo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pkiwsmwm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mlrzmrmc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2wrbvefty.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2iezchwty.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fiwoqabh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2nbtsaztu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jwzqilaj.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2zzgwzsrb.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2jltwuwov.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmoivcnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zbrmfiep.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mjuumnfg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tpimehjf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ymeaknyh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2aqxabnie.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2cqgwjazb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pjzrrmxq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2fllwbxwr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2knwtttsh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2cbpufarb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2jpfbkvgr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2susqkjbm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bfncehwq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2gakqxasp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yihedsfl.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ecdieoxl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oytzjkov.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2yacgukys.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2auoljpbf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2axmunoic.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qzgcefzw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2chjjreew.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2txqqmnvw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2xwtfaffi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2vcrhtkjs.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2odygqbyi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wokkpuvk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ozosjqau.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2xzqowowd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2goobyrmx.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2xtewhydh.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2suojqtcc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kicvrqbl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2lgbzzhgj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2dpwvszao.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nockvoph.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dndzgput.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjppszsh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zpljrksz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iwbcyjdj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2roafeqzp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ezycaaas.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2vnrhratn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2decwxopz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2iwgluddq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2qujtdoxh.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2frsrblbl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2aizwvzkc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2hhnlmhdd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mdovaldz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jcrskxpk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2pxfuxejs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwvsobdn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxntlwwh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwqpqiea.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2szqknain.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cfamhuzl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kpvprlfn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2anqfiwvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2lmoflkvh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ejfufhxf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2irrzefhv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2idrejhqo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uutuwcek.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ernzqmpv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2siwmzpwh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2oxzdodaq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2owlxhutq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2hxrbxlyg.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2szgdfwqa.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2mbyxgqfp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ilvpshsf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wgclhaml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2uieyohyi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jrfhctpx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wubhyhfo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mmxugnqz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2acvskfzd.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2wnwfppet.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2lqcomeot.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuokjuiy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gtsjlgcx.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2amrrchdu.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbrclfl.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jwwhjjwi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2narnkzmr.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kyxkhuwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kkktwtbo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2olkwofhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quoycgea.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2foiacebv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2zhuacqbb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2xesbuldl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2fquqmcmu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2aaapzfrb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2eqpnbjnh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2waladayp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2iitmajsy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2opegkjod.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2lbqggafn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aomailoo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iuyaxayi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wtczqifw.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qyqlyaxz.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2jltfotil.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2zpnqaawz.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rzkpsitv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hbeeakol.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ynsrgelb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2lcitfbtj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mmtycgrw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wjanewwq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gkybkqhl.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2smutaiit.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xvvwmvcp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2nnhfezjv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mbwilwuv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2odskrjej.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2isqmprzs.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ijoohwas.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2dyeziosb.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zbthkcdh.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mxhxzhaw.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2iwopptls.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dfzypaoc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dtcgyfnn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pexdptjf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2blvhcklb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2uwznlwls.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mntxdvbj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jdpnrnqy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qmoqvemu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2nbyeiddg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dkiiptwk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yzotrtpf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zviohqjo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2opkilcmq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2nvknvhof.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vqkdhljj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2byuosqan.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ziqikewa.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vjgxkood.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzhelwg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pkoywniu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mttikfql.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ogxyknlr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kgtbvudf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsgpfxu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aqmapwxu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2urkixria.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gpgosnsr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2fbqjqxot.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kcdcxdlj.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2dyqgtcrk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2jpuwfvrh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2jahicicn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gugkfqbk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gtirbjoj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2csgdibgm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2quffkpmw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uyzhufbq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ymafevcg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2hsmhidof.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gdvyscfs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2omelrxhe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lyabrszl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lshcoakk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fowuyekc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jvudsshw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ajxntonz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2segtudow.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2deadymdg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tqzxgaon.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mphrdysd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2whtwjkdb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmqorkt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zufaezab.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2oaiefida.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dobfzzcl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2woebtyef.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxrivj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hfxxvllx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gffmnhnr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2thucmfsj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ddajbgbi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pkpuouta.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vuuoowwv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lhdsnchb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2htqtdzzr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2iszgklhy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yvdmbomx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hbnknfqj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2knbjminj.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2heihaezo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gtrcnbvn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2urqqtnkj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mrwzkitj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mhtephts.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wckvsuao.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2sayylwer.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfkpqjum.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvfbjvnr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jqqeldbv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gykvpddz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qjdujeao.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tfrhqeuw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjdurkwm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fycbrexi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xreeyzgh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdahqdjq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2dilrdmpa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cncijoct.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2edpnxlyc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dnygirro.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tvffostx.html


<!-- 参考信息 -->