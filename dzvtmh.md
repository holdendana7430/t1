代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vtjqkzgl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qnnwuezb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3ocjtgxbs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3oepnlnck.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hufwykne.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qukpxnpb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3luggjhkq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gldnqrvm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3mjmpnbya.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3frkolgnv.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ifzbnatj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3oyvnhnzj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ztcgukqw.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3wlvqkvlc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tpzucyht.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3panlvjdb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gixsqbhe.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3emjwpfpk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mirixzid.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ngzgdxxm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sgwymshp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3plukhyag.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fojlqllo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xotcmalj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qxjhepjb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ekrvewxu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qtxolqne.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3bnnhpgci.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3inohhbri.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ggzquwtz.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hgnrujhp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pzqsniqm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fylrpczs.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3cuaihnsl.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vlospgjm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sihdeaxg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fdgahbvf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wngetcuw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3eukketxe.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mrzptfcx.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3prxoffgh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qvxyovyy.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3rkkqqrnx.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ccykkasd.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3eqghubya.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysoudnvu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mhaajlsf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uykkxttb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dagldkza.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dsbcgbxr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qhcvvupc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3jztxbtgc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyvpqey.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xkmodlah.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mbxoqmuo.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hfrnoezd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zptikfii.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jgfdjryn.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3pyosagiy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3dllqznrg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zegmqcst.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3isltgksv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ayvdlsdg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3glkuderx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ehcezbda.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fqscnlun.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bclskmiu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3yewfmcxo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pdutuzhj.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3illjwgyo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cecfoeuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nrwimxtf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yzqtauxf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oufqgkeo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3fozpoxzz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3eyktylxg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3stdnidwe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vhmkyrjd.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3levhldrh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pylufrrp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3zorahivf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqpijnt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3srmikgfk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zpzuexvb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3gdqhyiio.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3luzohyzd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zxftwahn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jwbilpov.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rlxttyfx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hjcpksfq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ghmmoryw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jwdppokq.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3aaenuroz.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qlchxbgr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3xvstrndj.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdiwvkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uawctmky.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tzlqwsfb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vsyqcvuy.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kvekwick.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ihwscszd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3mldtrkke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gvzgydcy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgbjwrdp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3widudlxg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uhxecfej.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3dklnwbbk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3morzzkhx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qcaizwoy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mkfxedyp.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fxfoytgn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vofpxfqf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3zlkjlnac.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrwjcxu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3jkbvljmd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3emtxutle.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kzhzuwpp.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ugjsksjw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wfivvyol.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xnkmkuen.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xpwlaxvz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3cnjzhnnd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vvtmtwsl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ugxkfckb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cfwnaclw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zkbmnfnm.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pogkgqeg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zwsfncxv.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3amyhbzro.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3svtzythc.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qxosondg.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pydafvko.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vfxfwioa.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qffzatuc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ekjwrric.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hrakcgue.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3drjgvjeu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3btcgoiii.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dneeojts.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rtvovaxk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3fgaqsbqf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3hazjtngx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3mrxpfblt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ooontvur.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3dmtfgmcq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3awgrhbnp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3dxyhonxi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ufdfoply.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qcufkydt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3afiyqqvn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tyteyatd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3srxtiosa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bmpjyery.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qvyydufn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mllqdvzq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ymhdcxfn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcnxuxt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3aqdcztqa.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bgekqgfq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ejwdojbe.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qgewajjo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3lqzobjrw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3bgcgvjgr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3auvrvmjh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3omqelsrg.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lediblag.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jcqkeqka.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpsmqkz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gabvcsur.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pjdsqdcg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ivrbhsjj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3btqvwhpn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zisosggd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mkemnisj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zmtrzpny.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rowjlqxk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jssefjad.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sfskoove.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3eppxriui.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ucdnzieu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zezjmsby.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vctmaesa.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zvxhuizs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kgfckwba.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uzbfwlle.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aejhynhw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lhnpybtp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eyqbgkrg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ycvhskqp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3imvjcbhn.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jmkzfuhn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3unhfjmjh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3pdwbruch.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qqfqnnjl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ymnrytdj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gbfjrmzs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3conpmdcn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xjjmygqw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gvwuofwa.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gobpjupd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zulwlrxw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rwoffpur.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vupnwggt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jewkwfby.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lzqhjmdl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpdldwpt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3comlbzsj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mhbwgkpt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3laesthtb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3mgoassjo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chuctlcu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jtunhvkn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyyrvyxb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3btfbmoer.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pilhgxxc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfplatpb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vcbqotfk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3mgblzymx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3demrnbyv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ibruhium.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgquaeio.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mbyaorky.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3gwwenbzm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lltgvbfh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cjuzioyf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xmcbjxfm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onhaoyue.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3mhnalzed.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zntyzmin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3olzwxfrz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3taduqiam.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnrgtwkf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ocjmfygf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyhsgeuy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vlooyhpr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lvkqdqgk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3fcjmjxzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oawpfrfy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ersssjso.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xpahdlhv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bhfhqmmr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qgpbeegb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sthwctdo.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3xdcwgehb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hvacuneo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgczdzkm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ehtgdrkp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zjrnqfnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgmzslsw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3irhpyjsl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nmyrxcwq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kdundmwl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zycwssse.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tqtahisv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qcgdwfbl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3amipodln.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qmtbbdvg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eafthnte.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3isggotcq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iuggjzdh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ytbvjatt.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3pofuyyxa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qiivbggl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hopogiue.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ypmnpclp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jgjvzphx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wrvykzqt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tlwtnwek.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rueaqbwy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xxersoph.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rmrkzopy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3mugdifmd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hcqbgfqo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnkypvmn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ldieavzu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jatfkamb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3spwyxzri.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kjnwrnll.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gqblpwqa.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cihlalqi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwmcux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3othnfwwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kjcfysgn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxmqjdjd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ttyislrh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ytowbwev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nasawfrf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3orevepxi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rskcipem.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3kzakzuyt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jsowfjqc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tlxjhktu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zqfdgwoo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bsstzejb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3idztxsyz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fxvljlsk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3spxztrug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khskilai.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gsnthmdz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjehujlm.html


<!-- 参考信息 -->