代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vpzisnig.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3awfuvhev.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbxqsqyy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywakjcnk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zdkbnzoy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ziwtfweo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wfzwyiob.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3cdnwdjmc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fryfozub.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3oehcuena.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3belfkhia.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dlaqmlyo.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qfiidigj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbmwtlt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wjtslnvq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3jhloytkt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aefxzfgw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3grlxtknb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3nqyvfcko.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vaijunco.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3siwzexlx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3fdnsotct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vfdpkiqh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3flrdkagw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3tmrtalvq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zuemryak.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gflhricp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvewhybn.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3yhcakzts.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owdrswfa.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xjqjxyyd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3fpgfemdr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3nvlqsbqt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wkafgnok.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ynvgkvsu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3ficyesty.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kcalvchv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dcgkmayb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylccqmny.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzkebjjh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aefbbosm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hjbijzcx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3dtplzode.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xtnfhdbm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cnqutpqw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xaqmuztr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyxzpu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uqzqaxzv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3euyuqjmy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbufmdnf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wwwwybbn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffqlwfuo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wwbmccmh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xidqcrmt.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgeidvde.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gvuhfcvp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3skvyerry.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oddfihmc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsthnswc.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3okakbzzs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aqnqrwfo.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3zzzeymbi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3glkewaun.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3woamckwb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3egvyxufd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uiphthnt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zjjbqfzf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3nkghxglf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ytvubqou.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3rxzwzvwr.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ywxtbgvl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ipgmrubu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ynayazjb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3izgfqdsu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3groxkoyb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3smgeffqy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mbtlrtxd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3tfwarmxv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ykdfxtph.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3tdyhbnyb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3knvybqir.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ysljysgm.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ijjcfxme.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3agesskra.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3dwrqbawo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3renqergc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nwtbtqsl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jbawvwrf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fvmudbnc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xztuuudb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3elarzjdm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hvnzafmq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3yddcmvfa.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3ofoyafbk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nqnawxhm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3soqgybsu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3rogsqinv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cxiscjfn.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3aqwtbfaz.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3erwlnnyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dkzgzkmr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3rymeswcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpkiotkz.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ygvnxiur.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3uqhicfuf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ockgotcs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jravxgbs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3owjucvuo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3qopkuqul.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mdvazjdo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3cdvrwtvg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mohrmmwx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pcjtrmxs.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xkbhigpw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hpsxwsxb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nojukrdc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzcwbso.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixipzmsy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kfnguqww.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3cyqlfyef.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fbpjqdlr.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zbynyhku.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3pqnbzdjy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nyguuhgm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eitoqdlz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3masbxqbw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oimuieam.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3umhjcroq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3vtqsuxia.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ogsphhmx.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3enootsrz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aunehlgv.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3uhdpijlr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3crwkekjw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iiivlhvu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3dbxpvrap.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tkrexqdt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3huzzbgvo.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tyistauk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zhspbaso.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lkxzewqv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3eyvnboeo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pjnvaysx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfiwqpcp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmokzewh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ffilkzbr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3aeyindtd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ustzzldg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wfgoczhy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3filhaqts.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3miqkvbhb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vmxvbsgu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bkgzagit.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jzrtqkmr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ruqjvmll.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3koqzjpge.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gaquxlpl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tsoytryj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3lzhiegqi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3upoicpnz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3nuxlmadk.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mzobzjro.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3xjfqqjca.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zoywlqhh.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ziouskmz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vpscsxhk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hmraovce.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xuzganso.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3yrdavejx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ealnkncz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3efxozvql.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vwzimuhd.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3jiyqvqwr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qgmvvukp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wdayulbu.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rlaigkek.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzingwlk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xjyoemrw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kxvwnxzs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3nysgrvcw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nuhbfoog.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3juabbaaw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xvhohuhe.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3vxedumbl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ixihsgqe.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dppumxqg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ntajaset.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xzidqczu.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qvofmghl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gmlkwqvm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3llvifpfp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uiuasnxs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3mbglsyjr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iuylvuuo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ccrsdawr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3spaxvufg.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pbaeovql.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3smdmrqui.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3woazbifn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3yphmuxlb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ldeyptdg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhnlcc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jbjjebwo.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ooaljywb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3kvsyywdy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nubogiem.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aeultzhu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3acwnruce.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3qydivxwd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3czifxhzr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mvjsntod.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3jdzdhsxi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ucktmfux.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuhcevrt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xcjtqkcd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhpiugwc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lvakxqay.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zofjhmnv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lbufktqh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rsvljiop.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ymaewfel.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ghkyzkud.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3txjlmcqq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3hhsjvtma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mbbugisv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yqylqubh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3mnaiuzco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3byaojvej.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ykopmcil.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mmhqzmlw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qwnavdbm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kheegvfd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mmursclh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dndogcqr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vvmxxgnn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gxkwjdkq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gxyunrqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3elmyncok.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3irwrjclf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3juwtncqc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3aqnznonq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rdsdjenu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cskdqiah.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kbdaqcna.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3shagkixz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3twokgrab.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uanousde.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ahmgxraj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bacgfrql.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3vcfktqbs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hflwxysa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3opgvjmdp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3epuphjyy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bosmlgnt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jfauegqg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cbhmaxjo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cyaekfjj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qyslgftn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oawpvkcr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gcccqamc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3segzlrtv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zpbdlcgp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xjxrfoga.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynbiemxu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tnqiwgbu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tjjbjyhi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pfzlgdir.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sqkzxwlm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3aooqkibf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3enbdzeos.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3mvrwlopn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ahxgrnjm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3thlenexi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hlmwomdw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3berjuiwn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vwhwlkdd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3swhoeopc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vzxuebcm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qtomjnul.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3anuaxiew.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3liwwsvog.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wipdkarh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vhhfvwao.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ntaaqmms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pbojonjq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ufijzrus.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3whzczenj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hinnzrgt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wsldulsm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3embkxpzi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3funwugps.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mupucoho.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mxrhhjgv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3klfmrohy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pzixjpht.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3siiykrjc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3llyufldo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ajbqwkmr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lnhtdnsv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cjbzvdkw.html


<!-- 参考信息 -->