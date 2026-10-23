代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3scpkorum.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lmeaxzcs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qbvqpxjr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vzbgwypf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3eemgdvkn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ydiomdtv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3wrhjwdfh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3friyyztc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xfavcukd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3mxodxyne.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ewbelfja.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uhotonzg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fabalcjq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zagujdrp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3agngjrfq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gemruwxx.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wnnwdjxg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3irlrlinl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3roelhniv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3efgqozxd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3minildqi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ayembjns.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3flqlxfpy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pvawgonu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3luvahpwp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wdjnfpsg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rdmmlmrx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xveyejhj.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cjitthcj.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rxnzifvf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3wufpijsx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qdivapkc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zfolaset.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wyngysyj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yoirbuox.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3seljzmio.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fyqlbxmo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3llemqxui.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3plgkrbck.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mmqewvvs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dngznrlz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nebohrur.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cxddsius.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3pijololv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bfnkqrtm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ccdzncjz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ufhllviq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uiygfsqx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3fiqxrhga.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lqiaovhn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3koubmfzf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zvlzchhc.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vtyschlb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hvbhkunq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3wyykpkey.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3gudcsylb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3hdldnrid.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3hhacllvn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3itevuynn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hpvvhlko.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fhwggusa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pjgafofm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3qeoplxjb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3kcspaqdw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gmxufrpr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3oyhywisq.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nlmguchs.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ylcioagn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvtppsav.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3rcdotcka.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ytfgemax.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bflmmboy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jiqpygik.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zifqwftf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tlezgqmc.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3efnowgbv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3zenyuvyw.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3awjyyqvn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qvydpppb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3tlkskogr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3bcdaoxci.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ablculxu.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rxelikvn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iniezgmy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ubgustmr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3rdexfbpb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3mcsjrjly.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3sgifgrdh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3llnofhwt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tfkpxbmm.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3zqtzfood.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3wmxknbxy.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3nfsvtdke.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ogdxymbd.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oasootnx.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szlpckhb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3jegzadpj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fcggiqsv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fxtpkzhx.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wtyclstk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bvvwwmsl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3nwhobrpm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ogihfkvw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fdqkhrxr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cihkubme.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3assutwzv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhoqwnq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3roejdjpm.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hanudhrr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujkpsgka.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hizmbxqa.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dokicyhn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hdatridb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3xgnwnlvn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgnwhfp.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3jtizwzqu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cmetcbdv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3wdbtnxdu.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3umosnuvf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3avcpjbub.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pdskthhg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dzfvfyqf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hsvvzvdt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nikhlhte.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xmpwvhpr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3swpffsef.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3brgcafvd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ymhqkrlw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3imxwlmon.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3osbxqtpf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rmorvgli.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjfgffeq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3rupkkwqj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ctfkeouf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zrrynnvd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3qtjwcmid.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3aqhjhufs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3esipxzvs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3koijyimd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vfdohqgm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3hzaoeytx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3cubxanso.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3semykgoa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmgyckd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gevqjjip.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqprdxvj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yovsxtih.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3weuljkyy.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nggcfzks.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3aujnadkn.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3uolamhpc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qkribujh.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3adiidiri.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3krwivuco.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cnulmvov.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqbulms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wlplttjz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zfivfgyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hksxnyhe.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ljgjdkpt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3guckfyyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wywadflj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zcawvyac.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3nvutoxtn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtsuqgjz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zigpccdg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3lxxqytyd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yixxcvow.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uhhytncq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3yaheoiwj.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dmmmdsod.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3igdoezbk.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vqastilo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zsdfihdm.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3rfjfnfch.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3avisnxuj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3yduarnsx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3uqmxacju.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jbywwqnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3itdresgc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rljfcuxq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qecycqio.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cokbkezl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eolonjcq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3izimjpqg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3mtzqpaoe.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jbhqlvye.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3edyrehpg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3udjxaukg.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3ficrascl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jhkhxxqo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cmjxbhzg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3coguuedb.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vebeueqj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qufzikya.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3apjxdunu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zxqxhtkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lfmukkip.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvzogccs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ijeqengk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vdnliskf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wljzkscy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rwbhteyr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iwiruhpj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rpbdpahq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhigohhb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mfqcbbih.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hjjnuyvr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlgzhdyu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pzphglje.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmlsypfw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wnuxofkg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3exzablyw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3betggfnk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zcqhjdjf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3enfwuntu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3dsewetbg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kitwwfyv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nqdxcxoi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qddssoct.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ohrfmmxi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3oiqujlvm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3oojlzbvg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jzlqdiru.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3fsnjwiet.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xpqitalo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ghgizfxu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpuzlhi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3knfaybex.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rwdjolpd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iasnfjav.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ckeujsgb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3untznrkj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uolkmefs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zimxvulo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qqstbspq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wfqfojex.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3idmawwuu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3iuuoeayi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3aymbeuet.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cefemplq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ssaxiacx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hyiiodsx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mdtfqzec.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3otuqpnpo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rudukfle.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3sxxcfspb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fybmaevw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mmlsmhdp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zkxwyhyh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3thayunoi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ucgqshnz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fgeuxiaz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bfxhybcc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lhcirmyk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dhrlghmv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3csuuhvpv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dojkkyxs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3huxxevxw.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hyuazsmy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gjecrqvp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xoymzofr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gfdwrzyp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rzmhqwid.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kwkecccz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rwuozfgc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ndadimlu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qrntwxcr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ouawgbig.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xslexfxr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3abcczcxb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3buwqanne.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vxfhmfdx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzthyzfy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3swlehlzy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktylssym.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3bhaovltq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kbmucjhz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jrwypazc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsrvwvg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ggburbpv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zyowoovi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xcqqgakr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3fqwjetfj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xedchmaw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3oxkwnhia.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iouhhezp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wobptxrv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctaavmqf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3gthikwwu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nnhhvjww.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ljqsvabt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3usjlswqg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vsstordr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3exmeznog.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ydwzwwxp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3waafhopl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hyaecioq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kkjvhhir.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3uvjousau.html


<!-- 参考信息 -->