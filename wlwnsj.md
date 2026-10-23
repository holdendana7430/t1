代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ystmrtxt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qftrensa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3xguxpkoc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3idfzqest.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xdjlrofj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3lffqwrpc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lttczwfs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dugicvdf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3aqayejxl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tmpeqlra.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgpejpzm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jsetxvao.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gpuwmeak.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3cmqntwbs.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3reinekam.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mcakhudq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qbpdavyk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rngtzieb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3afgyejjq.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hvgbhmoe.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lebdjyem.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3fknbvryd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3iwwyqunc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pvxwiwcu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3pbrqztkf.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbzkbxam.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fqifalxj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xitwfyoa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3abruwjyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3kqzlhsff.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gcorhgwp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3firescrn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3yklmgroa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxsfhocy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rwxgpvrm.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzglotjp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqorskog.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3gcqveavf.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3syxbcmux.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jxlxjzlq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3gsblwlvk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dviquugr.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsrmwlgi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ofnblkrc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vmdisxgo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3zrhhhkai.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3jhgnuuel.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bkzvbvdu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sfuituzo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gtvbciar.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3twulmfwe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gmihzsjz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vczxnwhn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3felammlq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uhultcow.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ipzzkqtq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ijaijmrz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3juctkhts.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3wbfhefgr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tengdrtv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kveoqofq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yipgzuta.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3qdlfdozo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3elosuzfa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blhnxkym.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ukcsikus.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ujulrrmu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3enjrkhvn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3fldooovr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3kdhrojda.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3oprgospp.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3qfeispvf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hxxpifiz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3khaoqwby.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fusjzhds.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3efzijnhy.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3remxxtji.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gbakcini.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3pqpmtinc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3seuscvqw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3kiohsmut.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lckgmkqo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ydunzpkj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3qndoqnwm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3asxsrkyw.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3wgomzkfa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3eqbdqztz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3crzmxsmy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ovumaxei.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ujgqilks.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3usgywzhj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ydveymhy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3glsllbaz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3greydmyj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3chwvqhri.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3hsovbocm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3osvghxei.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3iikkeejy.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mveccflt.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuacoyoc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pitlkexc.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivjufqii.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxwsribw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3odpvqnvj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlfmkoic.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ngkiqfdk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jnrluyav.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3vqcqkchp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3piofjbng.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3eehbttcc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xnjtonhz.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yblrmkvq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3fmqytapq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3waqaeidt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mjnqzdcu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3knweucjn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdgybtl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwljinp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3znpqfovo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tvposdew.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlqrdvje.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3wpyekvxu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jnvqqlhz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ucbruciq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3eaysyaqi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ytoujyko.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3pkuhjmkl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3agxgtjfw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3njqufrrc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3acdwqebs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3oiowvtyb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3akgkbcjs.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ogjnwmja.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3dutcjljb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3dsiymjek.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wtwaboaa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3wtymfkjk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvnxociz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vowsrsod.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3dzhtgjsb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xvdxlbgf.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bwrhwocf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3szvtoyoi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3shlicpuw.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ifqwjocv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vuhnrjqs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eroczjbc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3scugitbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thkmaecv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3okslojtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiziyhrt.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xdcfsfnu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fatdaswp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ovrrmwxa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hivhulba.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qiqeynud.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vtubjenw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jdhscfvc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3xkvvunlj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nirdntrq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nuqlgbqt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tzoyzozl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3bklwezvx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cfviayls.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3twvppeok.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3trpqznmy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wcntzvxd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3lhisuiyt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3difcyyal.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3kyccqtis.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3njghvgau.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yvpmpqpp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3whgmkmkr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3atuefggq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3brjchhcn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cwqixfpb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3pwothdai.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bqdiamqy.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3giujoxtk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qgccpczj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3caelzvab.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rtqvelht.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3eznwragn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tkagqjbr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3yjtecwkd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3whbrxlmw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vbxswwyl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3msrclpmv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lzksphjq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3qwnjimld.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fatfsyha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lahmnknd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3pbpbwvco.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3knutqjma.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3arxqdivb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3izrnizcd.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3etllkoce.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xrnvnzve.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vtczahbn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yliycsdi.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bwljeraa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ebrmftzn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wtxwucse.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ytygxmda.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wkecrcek.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mrejihvp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ytqlcswc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yoebujdp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3xjuxasac.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3sgtasqqt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jbspgdtq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3icsqgppy.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qdhwvfun.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ubdqcghl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3guhbweaj.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3vblvqscv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3khynwsgi.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ycbxbtra.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bhwkolxy.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zpukaeam.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jbdhbuve.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3behwraxz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hyrqzbhc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3bwrrltdm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bjxvedhc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpxivitg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kwijgrnz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uglzyozl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3putlmjjq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ivygskik.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3snmvouqw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yxcxuxnr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vmmvgccu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fywpmloo.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3zlqfoyyv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gokkbowx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ziezojsh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3flrymtqw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mnsvrnky.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pqlknjfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3duvlarsn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vazfbrzc.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cokdixhz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gbskgday.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kzjuohbh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3brfjxnql.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lxwasavo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3eaoaebyp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3dmqopiac.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ynqkihfl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3banskvuh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jgtplhcl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3huahffnq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vcjpezka.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3sqssjfql.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zzmicsyd.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3xhluqhqi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oobbzloo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3mykjuttw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3beidgyqj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3lxxbvzvi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3oekqkkxg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3esovsdjk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyerbxje.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kknitaqj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fzkrdswk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dtapoblg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3accwrpeg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iobswpva.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fcioyaav.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zfvncegs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hmmomncc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcemgpej.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pujtalml.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ntlsioin.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3tyapqnkm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3apyhvocr.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3bfvhhhwa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3knvbrlpj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3hjpyjyry.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hzgrrgfb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bowhkbcr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3botvzvmy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fqiygitz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ldgabtcf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3djwnijhq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xrtzueea.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ssttarso.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rbivynij.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bzejpbcu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wbkiahyn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3zsehtvci.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ilzqhsjc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xmfwwggl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tuvtjuhl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nhfjwtho.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xvmvwinq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aeddyvfm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ovvmuwtf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3eclgyeep.html


<!-- 参考信息 -->