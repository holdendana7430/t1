代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2smatzkej.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2scqdupht.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hwhfpvrl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2aonfscqy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gdallcjt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2alflavfw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xvrrwura.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nhpbauaw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2shlymsnp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wuwzatry.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kqcnjbae.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sfikdvop.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ppdzqkbx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2acilksye.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2vqypmhhn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2chwqsrmo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fwpxyhsn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rsxizozj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2pcyiwsmh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2iqatjdek.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2geyxlyuq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2urrqqwia.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2viodslcg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2frlvuprf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mseztcne.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2viiuaptf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2fzoirvbw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iquyelgg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ukscetkn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2uatyufni.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ghkopriv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2mxxjdhoe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2uvlkzpcp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2higbhnxx.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wgnkvnwn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2uzdnqumn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2enottigw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2isdkatcc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ylqvczqu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wfzfcfwu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2taebgpov.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2borlbqtz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qerambpv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xoyaulbw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gzmafxmp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwsfzime.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vnuhbrza.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lwvivdsq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ytxpoyon.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ilmqtzpg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ztzqyvcx.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ljkgzyoo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2qzvkcpin.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2uceylpsp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2yvttbsxl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2cgrvbkjh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dfnmgkee.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2mtpobity.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlgkcxff.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kyskbiwd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2njwihdhp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2needrfsp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jfzeqdzf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2pyioasyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rpgomyir.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2nvadprjd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2tngdmcxa.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzrtwal.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2rswttynq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chtkjjht.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2cwuwnryt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hbxbjlir.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2oxfmvkmn.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2fobnlhvn.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lwgbcppr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wvkwitcu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vfidramz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zpyhvfje.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vubjiety.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2rubrvign.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ogxfjoha.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2bujudcpt.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2rhwhiceq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dbwtvsuz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2wlspzzco.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2xlwccsyk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2fdzahvkf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2qqbxjiqs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2vddwufai.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jxljapdq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2uvlrtiii.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2oabkolfw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rlpixlmn.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nqtmdqjb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayuwtqir.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdwzhmw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2crnavkts.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2kxfhaawc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2wwjzzvso.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2sldegrps.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2psnpwnqu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2sjsgvygh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2whtjrmkw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2bniqhnud.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lmqhdiyf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2scqfqwbc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wkijbhwe.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tuhhzzpj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ehkanphs.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gxzsyeqx.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2caxjoxle.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzefho.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2rgvxusza.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lqxvjtnv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ffzdyfty.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hagiyrhm.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2cklpsxmt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzarckl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2mrmceftf.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xbgfhoix.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gxqdofos.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2lwrhnlah.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rcieqomx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qhowfoyg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2foshuabt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ckzyeclo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fypfwnyb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2honnrlfy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2niqctppe.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kaxvycev.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2izkrlxpo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2scvakzpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2agdxnznd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2wduwuyxl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2dnrkxvgn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2weqroiaj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ljxlihby.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2dinicclr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ozjdotpy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wyozxibi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ooxmqzdd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2xkyrjnsm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbvxhos.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2shdzeffg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kxxvzxam.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kxndvvyz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsnarknf.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pkylmuxc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kxadzrhc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2juqccukr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2cusibgqw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2tkddyvhf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ujuefjjx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2gmvfrcds.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bshnjbex.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hanfaobw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsjphwxt.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jmyhccxg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozjwoazy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gxsvohni.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bqxtwusa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ezmdijfu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cprizcxl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htcibvdo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gtkufate.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2rvgkotxh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ndwwdxfn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pyanrlde.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vasgjxfs.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fwzliyjw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cqbbpuuu.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ocqmhekj.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ecgyvmyu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2omfshdcf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2riboartw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2pzkprqgx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2xknkdsvw.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nlinnqzr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2deolwwor.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kdvoiolq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nwhhnxql.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xwgxddfw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbjrxkq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bocflbqz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2snubfcgh.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2votkmdpn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2diixgmtx.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2efmyxzzo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ojgzhojl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmnayfu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xqspgofg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gsbwzpjl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jwufasuf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yxusemyy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zxqksmga.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2paofkier.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cunnynxp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rxzevcvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iekxmkpg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kykqwpqr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pgoblqcc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2wnygldqi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fdlntikj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zuncflcy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2setoudvl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhvkytpj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kqeramub.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wawljadm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xzltfdxd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmyamycy.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2azdeaoxp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zgsnkhbg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mxyofhab.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bsptlwgh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2jfsgqyat.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lncecajl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ednakwzb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2irsnrawf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ozghqhic.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtiyjmft.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2fzansxlr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vewogzfz.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jxyiybrn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2uembatrm.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hqolrryd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vdsosaip.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ijspfebt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hgfssuyu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nfffiogh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2akpjzysq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pltougdh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2vfmfslwy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xclnukbx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmuuuvv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kuxvaxna.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nszikbhm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jiaydkdo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2luizbdkl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jmigpycj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2bnpnkemh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2chuvaagx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rshbdmgn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ejnpbnel.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vtebeuhw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qvuyftqm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ddcfstne.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bdfuxvvo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyvqazd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bgqtdqgy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kitwibyq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nqxtpcho.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2efhtupqz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2filegjiq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zkxzeshn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jverbhey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ztflvogf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xphqtdly.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2udtjdwzo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tbkeonja.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kzxosnan.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bqsoixpm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vijsptnh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wiqtzvqm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2pwpiquaq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2bucgjavj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vojoyxec.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gaxogxhs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wqsdbtfs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xeqyeapd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmvasvf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnikyzcn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbjajnya.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wtiphgge.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oqibatdm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2owlqkxcm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wxxrzfwu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2iudexizw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2cbvtqkvj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2osxhysen.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ltnvqlmv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2emmbooug.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2natnqpkh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nrzyhera.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vbuxpsvr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ttahnjir.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tociefbu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qssslpyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bbvcjydx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wzzptuvr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2itkuyrxm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tdzwxtyi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pbfqvwhg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iinicfee.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2btsqhbtw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nbedfbby.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hvkpphxj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xnlynukf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mhwfuhcu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xljkhhly.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ocrrshua.html


<!-- 参考信息 -->