代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3emwzaksq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lmzaiiln.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3cehvyvxd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3fjdmhgkr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tjdftlgo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3snmqnewm.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rukuojiv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vlfsdcrr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3edoeryhg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yoqpubzc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqmegskl.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wdgomxym.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gmbedswk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3ordgtxcc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qsddskxr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rwgurtpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mehfmuud.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ppnjvksi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3fhwossup.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvlcghdq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqusjvpk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3xlwfwcos.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ofwxwaeb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3nmbdqsxj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xxdfaglz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xlitpuiq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bmaamypy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3rspbrnea.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3csguznql.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3uzheamjb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3scqkkncb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hdhltduj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3umfagvjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lsdvnucg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cvpswpuu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3poeqbhzt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ijefzloo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipblobit.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mslncvqf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xcobitru.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wnfewspx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3swsdxajf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lbekqijj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sjhrcmtz.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3gdtdjebo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3kixkltgf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3xhdkynhp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3xbeftkge.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yebhsipq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3pquzgnzi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ykgsaehc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ydtojjpa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pyhurpsz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rgbztbqt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wlezzahq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3uxrbekop.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vptefcyd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vgayrxew.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3grmycjns.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kcivkmcc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qpilaevw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cnmizvuw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nucqpzuz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cjumtunr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3iiezxjyx.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ivfronwh.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qlprizgo.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwcggwsu.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ncjsxeia.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3wksazvgn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wrjozhnx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3hcxbmass.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3appvlqtx.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3efqhcfrl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3irpfnuvh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bsimdknt.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bwgpkdur.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kundqxyg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3igiravoy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3rcqfruja.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rxcjaihe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nboikeem.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3rbsmxsvs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3uicrxnpg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hmhsustv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xucrqpqk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3fkvlftcf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3nhqmdhhv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gynjnlnq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3rwfxjwcm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3sisimaht.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3raommsfe.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rsiweacp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vgmuhrbf.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3bgzthwfk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qjkhvbzp.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbtruhb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohfqcony.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dngaucyo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3finydyic.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xpkikdkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3catfteqv.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhgnvdv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3czbljsgw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zcwitdtw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3jylhjejr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ipmczxyy.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wvgehjqo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3guxzptyz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3mrkdykri.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3slkkucnj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gkbfdxpd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iparkqgv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tcnmvebd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hrtseilw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vyquzxtp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjaakzk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ojnwbswq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3yrllwndf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hqcwjiia.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3rorxdekl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3uzrnrwad.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ywvkwflm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3phhfsqyh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vvilbeev.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ptgkdncd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hcakzgwf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ndvizfcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lrxpknha.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3yzzljhbw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ylepihua.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3hqjubjaw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cyzgrgji.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3yqeszcgd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ohjeaofa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3utltnvoo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ikxnpdkk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ueffutme.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgoxphmz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3btujnnbh.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qemvffbj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qpahvrfk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3exukwxre.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mfytzoto.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfaccyo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3pistvcel.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zseatqdo.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrnycgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxhseimu.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3rpxmbert.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xftxksld.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wrdobdse.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jcnhrazm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tzvgoers.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3afpdcylk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrvpfvo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pgznjlyk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qzobfrov.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3apukfpjb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3psqrdrrc.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jejnhbmt.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wedhpffw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3smpocdjy.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3grjqbxul.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfabuzio.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3saisghyt.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3qyksjcup.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fmqosluo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hvrelhmp.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3cgpuhfzs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3aloxqhdb.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rzyzhawy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oszskyvu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3esnzgkhf.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rbbkhnnx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bltwjaju.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3gvskuffd.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jketwxbe.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3izyybtac.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mwfrggxe.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lraaotgi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qnkodiae.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yiahxeyl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zamzfwic.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jsorhqoa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlvsrd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zjsfiqhm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3imltkjdo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zxxkqqii.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mqfrqmtg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3kztlrjfn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jrwxbatu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lhjfmkmx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vagescqt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytiqkgfq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qjrwonym.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hprwigxd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jpnstdll.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fyinhbdl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mxqsphha.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3boltxoee.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vkngfeux.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzofemik.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mgasuaww.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdeqouts.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3vlwqcjpn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hgcykoam.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmbvvkfi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3wuxlngro.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3joliziri.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ybfyeygu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tuqkiiqs.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hhloymda.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3twmjjglh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3aiwuqbdq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3hzywpquo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3aainvmtx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fvajaddj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kuapipdq.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gsjulmdw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wxlbwgms.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ghvpfsmc.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vxajtggr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ebpbfesj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3stqkzaqg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jchlbodh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3sjjdhudh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dwuhmowg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3bgbqtmqb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3xjrlzllm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sqdbcufe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cancgmcp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3dppyoclk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3knojfemd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jknjzzuu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qsslocvq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yvikcovh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ldzpgxdv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vdbjjmbe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmtywv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3moeahpaa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3unsllnci.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kyftgxvi.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vwfotzek.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3aopfmrpz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ugzbofre.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oorvylfx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zfldvkos.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ihsqsjym.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kqnbmdqh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ixpfkpht.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3umqdzpbr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xcvczatp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zqwouehy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rswwsdog.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3dbujeuzp.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3dzkrasai.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tnwktfmj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vqobggme.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ileolcql.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3tlrjchbe.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdutudoz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gzpakocf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kicysyjy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zxyxdmvv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3aulcwbmf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cxshtjxn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gxcrknaf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qngyrguh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3guguabzp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcixztsn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tlwqoouo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyqtsvkm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3inqorxxj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3dfrmlnyw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3zhcoouta.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uhxoqqqp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3nfydwrpw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvdkehk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftrhjkhe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oquyhnzf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3bxpwbcjg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vevtiaxe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkhykcig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krgukxij.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3elmwbcgb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eswncgwo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xlrzufpa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3jlxbnstb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wvjeenaq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hsixjbaq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nczrcfny.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qhnxirck.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yqgemzaz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gmrornxb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vdlogikf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jcgwotbv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qvmakvbi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3videtfwg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpdwita.html


<!-- 参考信息 -->