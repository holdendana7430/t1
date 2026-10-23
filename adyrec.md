代发 wailian999

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3eetjbduf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yelsxlcq.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3evrenube.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eggxydly.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vtxyuowd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3yjpqihid.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wzajydov.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3febyecvj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3vrksjdbg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hguendmt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqlwfezo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vjvdbzrn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mhfrgixa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xepefbgq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sddmioih.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jrlxwwpr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3apzexqii.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bfcnegur.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3qgpoghln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rkeeutkq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wprvufie.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3urasbfsw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aodhtgab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3icwbdfgc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ayzhrhrn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3vklaambh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqdkniq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jiavuipw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hhrqiijb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ejxvtwti.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wmnpvjll.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3veaktqru.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3aotxlcgs.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bvcvfykq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3nilwgbof.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3euoooazp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3exymwcaj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mkbqtzoz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylbonehp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pppchtgv.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gjkdbqff.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3puoswyhm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ujunnlns.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3hqfmskjc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fswwasso.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rwjxmetz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tocdmkxb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjyruvs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjrixfs.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3jrirvcjz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ycbguwgt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3jbebghsi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rfngyekr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wjtpvigg.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jltzvqsf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzyesoas.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3nenveeqq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3mkwxuxuk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjvwxmtd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iuocgdug.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3gptbloxk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdhuxtfy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jclsdnyc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iltzcymf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sexnjpxr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3yrpdsuua.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tnxtpsmf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxhzuzts.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3brsjytsf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eksewemb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3vjdteiru.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3lnuufrxj.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mafqvpow.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zbpclcdd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3oystwuhw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3cmmpbzzd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rvtrooew.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3mftixwks.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hqegczgm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cpqjkiud.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3vkcqbplm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yynzzagw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xkygjvhh.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vtysjgdy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3dfgqijbp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oxgtgdpk.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3suerylfu.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3glxwcwlf.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ihlnqmzq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oxqyjesj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tahvrnob.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kdxahswy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kpvrkxme.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ykbrahbk.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rsemxarb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3rafxrqll.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3krgzypir.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ntssoczi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mwnytded.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ohzswzix.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3cfnumazv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3krfwvqwx.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gcoxadaj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3repivshs.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xwrjwezn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qnxrxxns.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lkhrooeu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qopkskfs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3psjnoqdu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hpwgxlsh.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3khgugeie.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hkaodkob.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3iyjlinid.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ipmvabda.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txyyjnya.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zryorxjx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3uydlcfqj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fzwztjda.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kiolhcyk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3vcxlmxnk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3udfclenx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ewdhsbbh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kkorpzjr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3msxdqkyw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3fzmdhtnz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iepikmez.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zznbknrf.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vysrxnwc.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eujzbumt.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3daizdqvs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fwyylzuu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3qwvpcyrq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffthqxes.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3okmcddwg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nalpxmpj.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3yfpamtzh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3uhnljffg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jgffagml.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3tjlfzbwz.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kvomioul.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ejtexram.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ywtafnif.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3tiqmqert.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ogqfriwj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3twbobvcl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3pbarngpl.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ntcsblrj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3iywubmnl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hilglxmg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3siiywmrw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3sszeyafz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3vtnwlsvl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mmywclwc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ukrhtyqj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dzgmbhny.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3efeimkyt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3oiijrvvl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3enwtyfce.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3myiwzrmn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3aktvbxkr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3xwzkncwq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ueatestk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3ytwobzvg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xzjdqlzd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3tlefldpo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3stntvend.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hacyrzug.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edmfxqzx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sktpteye.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncegcgsk.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3radkccfy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bcgdxspy.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3sgmzzqjl.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3tsziqvwx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jbuvxakm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dlprajoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkfgfnos.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nynohghc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3reuurita.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nkhofwhl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vnpgilwj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ctlqvxbc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jxvboqiq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3midubimu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tiimzltj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oyaitvdt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3auizrnzy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ntkpkokq.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qvagtugr.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3nobqauee.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqnerkdn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hkgfijcq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fzanwztb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3amnqskhf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3inzvyowd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xpinjjfd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3myxwgzoi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uwsadqxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sjutbmwy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bwnwkggj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jetggarv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3krucaxkc.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3sewhhefj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ugboyzos.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3phvjplyc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3saqvhopd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3mijmkrvg.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ssailnhu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3ntxiaafj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3mchlopbk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3paiyunim.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3povounrl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ztvsgltk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3avkpknwi.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uvokmsin.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3skgtyzwf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3azofbrsk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3uooxujbh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qadqpdzd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vsxaxkim.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ieynzidi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3imzpmkor.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3pckkhpxg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wutqasbq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uzeluybd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3arbwkzuk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3htudhrjk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3omjipctg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3arudaxhx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rjbuzkyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgjiicqy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wysrfoth.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ywyetilv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3licvdtzf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pywnibbx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3opovamyj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cjuljuwi.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gmhyavqv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rcqlmdjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3eejwvnwm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tmpirpnp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3chcdibam.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3jcbnzmze.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3hhfevxjs.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ttqkrkvw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkboufh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jhoaprhv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3lkyxtzbu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cfdgiwxy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3imzljjxo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ohyonpog.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zflfzvks.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ttievcca.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uwysalsv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3orevgmqi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3fssjisio.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3zmrrodav.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3dqcpapkw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3bemrkfcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lpxhoekw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lkupjsva.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wjobhemh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rixkuwaz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zflibzef.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ifvkxefq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mtrngpab.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hzdutsiw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3icqcdkcd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3atrymtbi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3duwathny.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3injnsbzb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ivtsqxqq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jzpsdcha.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uhxhykia.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iupyoxif.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ubqehpxy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ngogwcah.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vgozyuaa.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uzkqbdho.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3flawpdgw.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xqlbwyku.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rwqfhqzc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zfpzbplh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lfprutif.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nkhzilmj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ktpkrwir.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3zpymwxxd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ehbdjyco.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3thbguqbg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mnzcurur.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnqcpetm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ablvxytc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qfdmzpap.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3epexgqlh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mrongory.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3emxcsnrx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3szknesss.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zqxkjhgq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dkrzxdew.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mrgwsgqp.html


<!-- 参考信息 -->