代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tveepzow.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3tewjyanh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3osulicme.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3arcfohte.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3krfnvkyd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ygtgfhpe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3tcscfsrc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ggptcpkd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kdannoeg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qkpvkzgw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gfcgqbxz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3mltyphyq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3eopjursk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3agknoykz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3phrzvdsb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3uvcbwiaf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3jlioykhw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gldujynr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jcbrzpqq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3izjnnqke.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3tjorxkfv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yiwmuybh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3htzubxeh.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oflivmpk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lkenoted.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gjawlhaf.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ymhlylci.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3oyeitkkj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mriuxdjz.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ztoyybts.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gsrtrzmb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3nnqsphax.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wtheskbo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vxfhvjsw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jtaxagye.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3slldundq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3baxcszsr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3gcxmhfim.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3szminovm.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gcvoenkr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xdiijdlp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3okmugrwc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3efdcyvqm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dyqwwhfg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ifavpxmm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pavavfqo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qlbikypi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uhleycaw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ndrvjqos.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mrsnglto.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3kixvjlfa.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3jqaacluh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dkvjcouj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aupmfcep.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wngdlgne.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewnbkcmr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3khzfsvua.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3efsorjip.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3hwagbvdd.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ugnfpcus.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3rgrlgscm.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3sitprksy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3kvyoyzwi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3njslnfxu.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kokehwxf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3aimzhfmc.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3zoogjbpb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ysjeqkhm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zeeyooxp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3eqfawvii.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3kqqrnfkg.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qzuvlgsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nrmlhfzv.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3wfuuodrx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3churoigb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lozgcrmg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3vespalmm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xpcgoaaa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3xlrnoyrw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qxjuniyk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vleccuyr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzzerrhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3rjntvndb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vtaefxuy.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rouiwlwn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3uxvxvvpc.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3wfvgedhm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xphnflav.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ayyziqbt.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3fetrzlqh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3kbayodrs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3avimqbcf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3koyiuftg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xsdukmpl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3cukhczns.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3spbfwfpa.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3wiazvatw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ladyjque.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wxylzars.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3plcubfqn.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3txcovjfi.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3paraizyb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zregnzwy.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fvcdhjya.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rdhgoges.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cdjnowhv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oqarzpsv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lppwomxp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bwuhygyq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3oefhwdjv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3swikkqzb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qkocgmeg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iqivmall.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cdonhxql.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nylfhttj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cubhttmx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wsthstpk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ygghiyja.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3nxlpssxv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3icvshvtv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dbcedruz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mktcedhx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jsyujuis.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3fekiofja.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpjpuruw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jipifdtk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yzgpmyae.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3popcifkw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqbuabm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3njuyfmmv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vmwlsvwl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3naisdxox.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kumilhhx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tjjgigzx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ottjnuze.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yupsnxme.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gyxsfgpz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zxbjetzl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3kitsnndb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ufgchtqg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qdznamrc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3toiohqvd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kjqqeqal.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3wgymnbxt.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lrpyeeum.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbzhhzkf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3apbghyga.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pkonkrmz.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3oqyuzflv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vdtkbphc.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jrcnnlzb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3pxsmoftk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chfqhwkb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3lhybtfsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fosaiqdl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ntzirmqj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3yttnijvn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dgjfzqsa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rrbkhrqv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3gvhleblq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3dbuzqwmo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zbuqdekm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kvntdwnb.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lpjfzipf.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gqqszkwd.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hqkrhixi.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3exbtsqbc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pwypnyih.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3shqwlffb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3acnjtiev.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3wgmeybef.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3sodnyfcl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3aeosasok.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nrpvtczz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jbwixxxk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kwwyutwe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wcfnftvo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rrkdukfc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sjtgnfbv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xyzhzlqd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bttcmiow.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wibwaymq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nckyimgc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qejcpstw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lbdrouei.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xgiodeod.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cwbedafn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wltattdu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hmwfutln.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vhgmvkpf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3frigdnfy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mqonqvfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wrlbhakz.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3xwzqyhlf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eoneabgu.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fqsncwyp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3frzzxnee.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3uruefwoz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tiljbhvq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3axhoivps.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3szwcmful.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jipuslsp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymxcqbmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xaugwzxh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dmfgibya.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3waoshgro.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3zfhqqbvg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yphbtnqm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dvpcbwhh.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mjebbfvi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uyynvxyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gvlmywwc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbhgfgfe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xfwhlkjl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mamdicfm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqymvksk.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vzmkatjz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jcfxvntv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ztrefzrk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ebqjjika.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3anaznwuq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dynynbay.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qnrsldwa.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3npgrlolm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3zjwmxpzq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lzcmvdrh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qezlkvsp.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3zdagqcgd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbxwlnqg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wqpafkbi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ossbyecj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ggivxivq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iuejacyu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fsfionov.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3krzsobyc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmdgyyxc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ofnbvema.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uocwgqlk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qmqthzkb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tltdmeom.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hbgaiwzu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wbtcidnx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hslcwweq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eyyvhfvc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wfmefnxa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ewcykkpt.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yukhejnd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3youkaruu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3futlwzzr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mbrciktj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrdnunbd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tguflryk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qcfpzwun.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mnzslitw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3olodpgho.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3anpggheh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3spiucvdg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3swqbtxcx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhawrsxr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3afoutsjg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3adqbekcx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gpsguzms.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ebjcgbgp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3zemzbrbu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cpeyzrba.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ktotkaai.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtlbhnes.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ormbsgtu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cehcngou.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3acdcihza.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hpyuvckz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvbvgutz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3knakubmy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dlpyqizf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jfzrtkvk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lvzrgcsj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ywxawwfp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gungkbst.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qgjcotds.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3erbwznit.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3esdkhfdx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3kykiihub.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3btvjvzcx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cnzkjesz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pnfqjkyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3kpdqvcnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3praoxsgi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ofrnodvm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fogsqhxh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlygcuq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bqgtlftu.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3eqozvagc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gxpsqteq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ryyxuqeb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kkbtqgor.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tdotfjbw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gghamjdj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vrofsntl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3iflpjxxp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ruwkbjxc.html


<!-- 参考信息 -->