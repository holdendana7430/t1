代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3nnfgarei.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jhwhtzpj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zvllyust.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3ybyfgofh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tzutpznf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3bknigcoe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ujeifque.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ipecqdis.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pedokwwg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3scykgnds.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ahrcwkks.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hojtsfwa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lgwwpqti.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gthhiuks.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dlaolchq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3nvgnvxuw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rniksvok.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cmxknftv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3idhtnsze.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3cuswhobf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mogvrcjh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3maecsowi.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lgkxjucd.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sypjvxmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3dioddqsh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3numvjgps.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3guxcyufz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gximnnsg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aodarmtc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3uyrgqiho.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3phglqewq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3tnlhplcd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3igjecojn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rvviqthf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3psqdfteb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dbqcnxdt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fdbmhiwc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yvgcjuuc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ydzktlbn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ptnyztaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lbfbvgmq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mlmqeacb.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3nsveuryj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wawdjbne.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rvnntutm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3togucfzm.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3anmrppvg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gxdyzkuo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vurirsai.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3vjyigfep.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgmyazuk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3pqepeuci.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3muzjwvfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hfyulsib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3yjhfybzm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3sgbrzfrf.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ufkkwiib.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3dylslstc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jqascuyl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wemnwtfw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jpjuszsz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mgrpaumu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bqgfbaxh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3fkgzrysy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3smrksivn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wkppdjzf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3cidauspd.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3stglzgam.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3yklvlheq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lnrvcrvz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3xyqquslv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3chnyoboc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xeuwefxx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vdzbbrqg.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ziaxnmbs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3hiyoywlr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3hhchtzhy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3apcahbik.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wmkjkrae.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gbahxkyu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tosmrnxm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3phtnkhtd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dakmhxdt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cvlolcbn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lctvfpyq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vgekpgkn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ghwgitil.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ylqqwlik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3muhimxno.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3gonamoch.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3yfgwgmme.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3borlnfce.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3egrwnbzb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3jtfiavkh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rfetkvzy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gceuagzc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3urnywzya.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fdqfshuc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wysrqbut.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3drhgkxuv.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3djivgljj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qjxwxwbd.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jitgwpix.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dysnrtbd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tpcicfpe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xeoonfag.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ulpojtpf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kivhpjgo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3utzcxemp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3caqqiqlc.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3emrldvwf.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kpzjdpwi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqyayohj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ztkuhzar.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3vvmcrcrz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jykgcvkm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3faljjdem.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3aqhcnqzf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3iligszxa.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3uvimnbif.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3zviaufyd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mqanydhi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmkwyddx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3epbvnhbn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrmyqlxv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3lebnptrn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipayhsos.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3wgkicirn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmwisjoz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3urbupupi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dwvkdajl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mgmzgqfp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ikpizkku.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3iliausap.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3dcwwnytw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mvftakjz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3bluxzkjb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3uaxcezuo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3rsqmprpt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3qhcdcssl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3onnlevpf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zjqbjofz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3aubbkwel.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3rivsdghf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3fzcyzbuk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kzqlhvbz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vnrbzcih.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3arvxzcaz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3tzpuwrad.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3vlgabvad.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3beobwjjs.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3usgvbcia.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qvrmvmcg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yeqicuvw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pehuargi.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zckcmqec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxdcooff.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lgmltuhn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhmifaxo.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3grbyrvzt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3psyqfcvh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3twgarpwf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ifcucpxn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qnopyzdv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3qrzyupoq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cewdaaxi.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3ifgufazb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fcimszrb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edzdmyuj.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3imhcmara.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lbigtudb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3utecrbmm.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uilelale.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uxokvsum.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ufjzprpr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qxqvouxg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3qkikvdys.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qcvprlyr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tqsoebee.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3brlmwbbl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3eixcvuld.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3pfhqocwr.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3muxjricu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uulaavaf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bsgcsafl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yncsntrr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3uzfvkdqo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kdopdkyv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pxdzjejf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yeakcfop.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kzgenxsk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nubvjfik.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3bzhuhaqc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ykzsngeh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3kwngthmh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3oelsvgyn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3qzvhgyga.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kdhofzrr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ztzpdcld.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bpdtatlp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nziwidjw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wrwqlipc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xsalogdf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hteiyqof.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3djcxwoti.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxpvjyyk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3hgywgsnc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fpagljkw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zmrtghpc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ldmadlvz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3asmkqqkw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3iqxldtsf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xkfnlswi.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vqhblwih.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3pgxunaye.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3chfihekq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3reotyfvr.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3onitdjue.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3tsstzaty.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vblzbfve.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vzwrhekj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nrzemlxx.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qdulijbm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3voogkohy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3kxxepspg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3tiuqyxio.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3knkvzegc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gmplmazy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jsyzazui.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pdbejbzn.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mrnjdbjn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ufogpdoh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ywxnciaj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nlhgzjez.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpoquyin.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3stqzpiua.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ndluxedp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xyujnqzf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3elsipteq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqhxphzu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wgsreedo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zdxfcchl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lkdcblzi.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3dxkqxbuh.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbuomaj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pexmkvua.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3tqkptdsk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3zmuayxkt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3fukxqntw.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sklvafyb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gnjbjjfw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3boinqclq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qrvletvi.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jelafhyz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uxppdlkf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zsaefena.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hwqdzwkp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3qeziqmdm.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3sdgsylin.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3apejvplo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wcdemhln.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rdcbhfeu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3piaoicet.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3xdcffuny.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vtwsniml.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wusgzddk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3kxwwtavj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3dksqwasa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jjrztoup.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtqvavvu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxgaaswp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rkzihqfp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3veidjxbw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kshkocdx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ypwtjlej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nakzxrpv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3azxvtdtp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bhkvjzho.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bjpubmlc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dnbdkczy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3azdisabk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3fxwoejgr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3chocyqtw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vgrihcvh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jnaaafeu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kalsaqbk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rrxvvllj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sshzrvrw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxtucaiy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rvhsllso.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tinqishv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3krqignwe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ekhustkt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lgxyhaon.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3thamgnew.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ubdaaysj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cotzigav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yhrhutbz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3thzfcktx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xgmbyqpp.html


<!-- 参考信息 -->