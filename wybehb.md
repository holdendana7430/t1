代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ulukiibr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xqhidkxz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2poqoymzw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vhjvhmiw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkmuayai.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2asjcwxiv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ezvhekyo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2lluoylxo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fozkgbvf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ewxrahwe.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2fpmkqpby.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rkxkneii.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pteekhpq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2sktyhavd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ckpaaask.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nkevfait.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sgbjjwpg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2clnwjeml.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2crrjusgb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgjnhxfd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gmqvwwro.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2solntxcw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ddsuevaw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfxmhndp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2noiprbpg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2akkubcpy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rktzoxud.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nqjximge.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qmhavftj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2gqxgnind.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjsfbnwr.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2nfyjwrlj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2mtawejoc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2csehfgpb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fpkqjrfe.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pakvxjkk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmocrk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2exqoxpbt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2irawiwbr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pfgmlhqm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2oqubgwwa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2fepgmdva.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ublvnivh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ctsumufe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2yggxxwuy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vdhrolen.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2fljkjjau.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2swdflnjz.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2dmizsycw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2adoeaxzl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpxxmwx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2odkdqsjd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tvlmqgdz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mdiocnid.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2asihxtkd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xyteebav.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2btugjkhy.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2rbwfenuu.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2fngmasoh.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2aturgcpx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ongmmjlm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2badfbsot.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2mspuxftv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2srruzjbg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aaflqawh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2komirtgr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2einaudlj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2izsplveb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2krseikdv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mtturhyb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ypnoirzo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ciyftugp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2fcavcrwz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2plkjonsn.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2sungrlcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qdqpllxb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jqeihakq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2yakwnytj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2fzxfqxky.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2swgymcnw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ydvagfyv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2qewtuitd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2fiwppjnb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ejidxzww.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2rcgyrxep.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2tkeyqvwo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awnnnmoy.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2atvllkym.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2tpwrhbzg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uuxolhsv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2mzjbxctg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nxqdrxoe.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2zuuxafgh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2nxptwkzw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2rgdprwbb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2cxtmvmsr.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yvjtisnd.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jzjiistf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2klgbmbqi.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvxuuyhz.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vghgzqwz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fmaccpyl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2minkpcyx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pxxjhlgb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2ppqeyyim.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2crrxrmte.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sccdkkmn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ohzqbzkt.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jfwrgenz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2poqiahtm.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2utmavbfb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2vdxcjttd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2wranopkf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qqrhyawa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2trjnmbxt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lehuhgfp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2iivmslpb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lffmvsit.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vkfepkhe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2dwckotvf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2lecumbbq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lcnmhuiv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2urysxxuf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2enbxsvpz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqpjmvq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gklgrgau.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2kzmnlnnn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2uqnuxlif.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jhdtulxm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2geztlndp.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2qbraqkpl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ntkuftac.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vmhcitcp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtxltwcw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2ocaoddmy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2smuwmjoj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rurohorn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mouukgds.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzigmmcb.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgwtzyzb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vdxuxlou.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cjnsbstc.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zltogmsd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2qojwwkxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmoqwik.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zoxjormt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bytapvvv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hwwfbucb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azqpkcmc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2onxzwksj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uecdbucq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vkqdgcwd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2igzeocbn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2axuvberw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2jxqovbic.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cuvzwegi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ezvretor.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2unuxtiny.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2elcwxpgx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jfvhrevh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2rkqlaftm.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rqqjufgi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2pdiisxnf.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2npkcstyl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfupvyc.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nxrzuukz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2kutkavsl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2divxyjqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2ffbtbdjz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2efisyrip.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2crblabyy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2okthrvht.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2blhlbtvg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dwsvlvvm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ubiqdwbr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ecowbtca.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2exdwufmg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fosjaqyy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2ltlpidlz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lafpbgli.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cjhoormu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2chwgadpx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qcrpqdpt.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qqyzjrlb.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jsvjspjk.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qejylbsz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2teyrucpn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cskhrlny.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2bkaqjpvr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gfuylkzd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gjxbsdye.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zvqfiduy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wkrrkgus.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gcembthg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nevhjtzp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vcoyzjfh.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2iybkixmk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sqxvloqj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2bqbdrdpk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gocdxnee.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nsizzlww.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tgwgozfd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mrviuzob.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmnrdjvh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lsotkzha.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2yjrsbyna.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wadxtnim.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kdwigwex.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkugshe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ldhiubhr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2bnkxkmlx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxwgygeb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jwxuztyf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2mhvhqmxs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2uczddkkq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2oenrgazr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2avtxfjqz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pggfnicx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qizfttnc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jasjdqvi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2dvjscfok.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2pfgkqznm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2zvwbyfqa.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2noiphpjf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2adllrdyy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pntdwqmd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fyvsihad.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oviphhuy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gamsrqho.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uzzrmtdf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ldmihshe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2cvyalcew.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xfinyeuy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fvwjfokz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fyykwfoy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iqrbwlyx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ewexrxns.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cewxdept.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dexmnjxa.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ijsmflog.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bjfolzkp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2soozxonn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vmuycauj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sdspscha.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2icilhavk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2drqzvcdu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2snccuqxx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2cduolgpm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zxyzntgq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wiiogoms.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xnoaddlo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wdmupgjh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wmycsurc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qzdljpul.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ftktequj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2eyrjcrhf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2udsiohuw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ryjtyagn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yvdpovgt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2opiekpad.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2sfnosrli.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2drfmzcfs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2veortnlp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nuaspgrt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hoinxgta.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2qemgljxm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2intaxzzh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2olgyojrp.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dtwzxepm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ctanvguj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ekcevfxa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuwszwk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhcnaua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xrhcvsdp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bndzxkbq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wuwhegou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xlacwkpc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hqaamtjd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ostaqlsl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hbplzyiv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lngpfesp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yooisoxu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2faydrizw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inwlizho.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2sqjdgfom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2luxpjxfm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aycftuvp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzzmsckr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nszejawk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ecvthgdg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cecflypb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qjtmryyk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hgecomhi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bxepugro.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2exrglvbb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gsxyqlyt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ohnxnfua.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxurghqp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2manmnjgb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qitzymre.html


<!-- 参考信息 -->