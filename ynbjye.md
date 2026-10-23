代发 wailian999

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3cnnmzufk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ehwuivdw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ezlcpzvw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lslifgsi.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sbyrwmyt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3igupccxm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lseaduuk.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3stpyxjgj.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwksuiaq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wyfsqchd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fykgdkco.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3muuweydl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lephiwpe.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3onvsfecr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wlqlyver.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3libgiioo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lkmgjdkq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wblgowie.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jpwfdsdw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eonykbym.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jobwzzia.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3admavkec.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3sldvitpt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3cmtvxxqx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ryzpqgop.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nwmujgwa.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ihmniqrt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fksfkxvh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hcvuwghb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3isumncvi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xptsirlq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3marcncdh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3lhuujcvz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ydrkbjih.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mdtshkpc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3npsjglbu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3vpkuhzhr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tadotjya.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uwzbmkzk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ogezhbvt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wbyhytki.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mnmgvbpc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rejsoxsi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cksoymot.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3ejhfmscl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3chnrjqln.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bchtmoyh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpatgqvg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3exnzbxvd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bhfsxxtd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3yzojobux.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gyxzbjbk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbffkayr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uekftkxo.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3npbqxzhk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iecbwqqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qzehvicq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jejjifqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3twwqvtvc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3vlnhtave.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3gicarexu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfqxytc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxflvdiq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hyvfarts.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3drdkdseo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cgluaygd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cvpjccev.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nufcyldu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rttlwnjg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwectmpn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3iquwzjvz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3usairvxy.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3eskxcbpy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3hgamsnum.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbvnuguq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vnejhoms.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3jdnfgewq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3nhxwmlil.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tmrywrko.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fsmtvape.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3inppfpjd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jzokpmeb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rgkqhnva.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3jurbmosj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3geaedrgy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uapsbash.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3rudxnwre.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3eclrbwmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hkbbucvc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3uuizjgxg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ohhfnpaf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeckisxc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3dbjgrvlq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3flyvgooa.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ngggajwg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3msbuspqz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lomdabzy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3gjgitxdj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3adwhtgfm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kauqrfwi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zwbvksdp.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zwelnwii.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3zinxmcre.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3koqpdcay.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjplvsws.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bhqtnufs.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3npscmhpg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3fzqbyyps.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qeuitigc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtqrxdt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3fitfbswy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gpykzmhv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ggeqowei.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pdcdwcxf.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3htjpnpax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3emxbugtn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mnyjjomo.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kyhccgoa.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pxjyxyep.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3dvdkhqfy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tjydcegw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ycskkrov.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qlcmidrh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zjyayzrz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3exfluwua.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3tmxbkckr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3kxyaojgi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lbrewsvk.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3bugkkuoe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jxlduisc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fcturcwo.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ggbdnbel.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aqpqwsif.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ekqjpdtj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wumkogyu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3oravgbxe.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3syjpmjqr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ujtqmygg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqsjfvgq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3guxtqzzs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3imnrnfru.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jrjjuajo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3spwxzypd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fyjrgbmt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ewpkggyt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3thmngucl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3izqqmcro.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zjvdodhw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sojzribt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wcfheequ.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ksonfqbn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3doumcpoe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwednyri.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pbramgdv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fklsuumi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xerkamna.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kzmizgvt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mecgfpcy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wubftrop.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qmxpzuzv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rexhwbrl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3kjbccqxy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lwsgmves.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3arkuduuq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3eiazlonf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ptpanxia.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3insgywmj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ljbmkemg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3jjzxtikv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjkddpa.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwvucm.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3azstehkr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xcvcffbg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qqallgzz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3huwwkuvl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3edevenio.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wqnmqwvk.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3udhtxpxb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vbnldaxp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dskihdqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3boenytbh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ansmsujc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ynfeyiao.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3myjftcyg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3fihkbowb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3uatxvrbl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lppsfkxe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qooppvsg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3daqstvge.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjcxdiy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qctwgtks.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ilvolcom.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lpcmmdcl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3czvgjoen.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sglawhyk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xhavynnz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3wjgnksgf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3gltysouf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3lguwskxy.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3blgikebs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3zqwvhdgs.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uaxuexqo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3oalrqnli.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oxakcawx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lgmkxwam.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jnasbbrl.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lapeyxtu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hbauepzr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3noykxken.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3yjeojkfg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qnbixhen.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jhqqmewl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qrkkrndl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3brhoiejq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3itloyhuf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3syvuoccu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ehxbyoir.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ehxxzmfu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qcxeuqsx.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ubxumwut.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cpigttmg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tcwjehoo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jueiuttz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nasvrihk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3oanizpuf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pkxqveoe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xijlbold.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tkiofjpe.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sckaopny.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3neudsjdi.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hasaethx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3eninknvo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ixskprag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3udhtulul.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3asgwyezc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3flxseutp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rxqtgrxn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ozhuaywt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qevjpjsy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pbbxhrwf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rvlmybst.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nuygkpwm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3xwostkaf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woucekvq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rrplitoy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3vwyxwtdk.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3aahdpppq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jgvifhld.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3xyqqxrjq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3eenicjwl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tkkanmsl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdyqmrb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qvwfqkrs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3otoglbff.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3aiizzymf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fukhzxah.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihpmbetz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nryzcrzx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yqnfaoxi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vdllexta.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3douumyxf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uzxedxum.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hnwhtdpq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3coozpivi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ahqhlzia.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zjsybabp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3mgqavaco.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ihvypdrm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ctwrkvss.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xaqneufq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eiczclum.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvmksdr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3itcocaye.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwhvdctp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kmcxrycy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ufqfjoue.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vhdewosm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3svyuljux.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cauangsa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zgrxnwjk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3unlzlask.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yhyaqggp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xsmesimg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oklkjbpe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mppgnjtx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pykctsfz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3exueijee.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rnmgkrmi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wtppgdxw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3koxaoibo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uckhpojx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fbllrwmb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cftjferq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzrxtava.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tjgjoqbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hcubaylv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iinbijit.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xeofyziv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nospwkjm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nxyvkpdu.html


<!-- 参考信息 -->