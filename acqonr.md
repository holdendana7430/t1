代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ogzjjwko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dauqwwbi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2yjvgpzuj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zliqyyxn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ndrynjou.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2dfjihkyu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2pkwjoycx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2cbicxydm.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cejwshwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tbbgppdl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ityhtpfb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2glahvxns.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pkebarnp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2eaxrvsrg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rsugvrnc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fztoxnuu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ioaaafcv.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2hwyidube.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2omifqitc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2eiuolgci.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vipvjvak.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uanxxufj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2lmbevqtl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tqszbupi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvstmpaq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pyzzlulm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vwxawgla.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2yqmydgxo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2hyjpcvok.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2vuprdtfy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2omovjewl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zhwcutvg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2knzbncml.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijecsdkd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xbnwjtza.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2ehtukeix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2smvxsvbz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tgzdnzhh.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qwrvfspb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2opsdhbqm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jdvpylnp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2wwsjopmd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2oalemfiq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nghpdwzo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fkwvakyv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ydqizoki.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kojmplrw.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wvkmwhmu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2sxmbsusl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pnfmrzvn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2litcfwik.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2mafufbkm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ramgosjk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2liosoiro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lisnnzsk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2kyuoqdep.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2pkdgpibr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mbrkbcdr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2ndcgziwo.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2akhvflny.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2lbcluohm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2alrgltps.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2rpvcbcop.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oqfmqvtq.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2xluhmerf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2supbnlpg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frgcmzyi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ttsxztpa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofmlzdms.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2iakzcpom.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2gpifrsnb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gnscwuvk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2ciptkqda.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2kuzrwqov.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxzxyea.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ooagdpyd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2knsyxpbf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mtcavlgh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2ulaahlkp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2oqnioola.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xegmabgl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2atghtamz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2zxbmmwpp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2neauewko.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2vdixrmlk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2fiszvyxc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cqwyxvzs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrmbpge.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2yacsujwr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2dfujkvyt.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdeznncb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dmbivycn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2utxcxirp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wpjlqtrt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fhfbfzug.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wbvgbgah.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2zcqrhmqf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2rkqxexwq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nljkbjht.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2escgrkvg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tnpljsic.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2oqblhjrv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nofvhvhs.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ptgwuycw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sijikqod.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ohznzvqq.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzuifpf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2hroscutx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyvidcjr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2irwknseq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ixhjixtu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ktoyqlhs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zehwgdai.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xkimzwzc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2krwhkwmg.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kyonudcr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2udhlywze.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfsxskc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2dmrhywel.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhnialw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgjxemf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xbrnlapi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kxwvloyb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2ibapeksn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yimxyree.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2tiaucnzw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2owputqed.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zdlijmur.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2etacnvkc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2radvnhzq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2pciuhrbt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2absekuay.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mduspwak.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lwbestix.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bonjsxrm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2osfarfrn.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fcuifgjv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2quzovdye.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ojietvez.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dashqvcr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2wfusmvvq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2fzawfjli.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppzdylyu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2djdwhent.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2zqddlotk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bsjceqja.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tijwvkzs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lskjnewz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2abxfwyfz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bndnbocb.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xsxezofn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfqcmby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmimwqyk.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gjntdjaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qpxqkrxn.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqkpaoru.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2filekitn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2krkmvtwf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lsoidnzo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wpzkrdfv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2efollngo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qwakbxlk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2krtadyfc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vrltatvp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2chfwiiiy.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ojlcfhpm.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yosbgjxt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnpbhvkc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tmxwhjdf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2arvlxzym.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2wttiwfho.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ezuhjwdn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2mlfflpbi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2usxdhqkq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2poxwutic.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cnbmkmrf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ssrrlsur.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2eqggjpxu.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pempkrci.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2wnondipa.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2bxsbuifa.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2dswtobem.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2opxbnwno.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2hrdobasj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nyguhnkp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2qcnrdntp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xqvrpvzb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kmrhwrix.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2pwjcpilx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xigsssrc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2npyaktrc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vigkakhj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bumlmblu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2nzuzuyuv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aqjxcffo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2yfsgyhct.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gohxgbbm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xfpssync.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2jgdotnes.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wtrrijmt.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2gtrlfnta.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uuednvrd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uvhjbfbs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pfwmutvg.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zfoozdpl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vdzfrjfo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2aketzkgv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2duytydeu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yswmqgbx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2asdvoegj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2lmqpushi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ewycpslh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2fkvxxehe.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gowdxkug.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2wkscvzil.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2oggmptlt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cqnvdqco.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2onvcgzde.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2woabiuim.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2btlxceuo.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2krxyjpvf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gjmmusxg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bvfzjpql.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kxpbtwza.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lsduvotd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mfnwrtew.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mvslqumz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2nbclfrrs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkdrgok.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2zldkfjzf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mpenlqox.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dqlvwrfd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jgrtlncq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezlwrhpw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2zupzotyv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sfcsjcgj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jlkylavt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2shytoiyp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mhrcyxxq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wewwijyj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fxesicra.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hihrpeen.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2seoplnle.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ecazvuan.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2feebfyyv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jfulkfdi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wpeddxqi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2omfuqjqs.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pbfdtygg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kwbkqgzx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptkgsqww.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zglkvqgy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vehmvuzf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iimmojap.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jvopxwjl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kkuexefu.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wbcvfdqt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sdqwshox.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pyuggzxx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2csswhxax.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2itmbhvmb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gvscnamk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2hitnddzu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nquzajpi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2buwmoitq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2sipwueff.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjwomrno.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fsdurlju.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgnmiok.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mylhmlzw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hfwhxcdf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kniqbfhw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ubtslcwy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tnrrviuv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2fkjoryik.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrprdqt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzloqxj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhyfmxb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bixwlpnl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hhlbpxow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jcudbqtn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rwcgwwfy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zfnhukwp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jrwfhjuj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ixkqhfuy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zqmtkrpi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ruuvliux.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gszslerh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vbedudjg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tssrphzt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vaegaivt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wghsdrge.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ktbdkqeo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hqzviakp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtjauep.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2efvfgkys.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2eqkjzbuq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ssxvvvmc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pgqttxzp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ytbiivud.html


<!-- 参考信息 -->