代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpiofnax.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mwtukago.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vxulvzug.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2jpokohsx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ivmkpvbn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qugvkqvy.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vwmcvpkf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2rcrcxjyc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inehzqbr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2gqqioxll.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zlxgbxvd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dmeawdqv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ubffojrg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gwjhrmqt.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2leisccvl.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2fskrcbaj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2jiwxjxxu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gkoxkaet.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2pymyglgx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2iotrmhzv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvyeubc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2zoulhlas.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2dghgxowi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hsdhxvax.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gtephvbx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2lepxjhha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2brptwuym.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2kdatxftm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2xwesrtfi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tssqlcyq.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2lwltpvss.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2gezcgbsx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ctaooxmc.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hyseaiul.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2rwhsghfp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ifrayrov.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jkmsslct.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2qzhnivon.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2fniyrfda.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2pjicabvy.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2gkwdavbp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uqqnpajx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2wzhdjkil.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2mdvjdlfa.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lwlvtsfc.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ugxtmnni.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrcnpej.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yaxnvage.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghnbdxpf.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sncmcrxw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnvpoekz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2wcntxxfn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2celdwfum.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ugzzuqeh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwdkivnr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2daclaqbp.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkzvhtl.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mqhrqjph.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2sggkztzx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pspbijxg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2jzibjmra.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rhlfpwiy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ilcigauk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2aifkjfjh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yajhtkrk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2sacorpwc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lcvzkohq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2tlekmnuy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2ipplupyw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2srrjcwht.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2xbctfkqe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lyhswilj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aoeeejic.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2rkycnylg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2laxnthfy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2mqloinit.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nuyhxjlk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xwtxoalu.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zopizteg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2aivzyhkp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2qlklukna.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2mczpczuz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2fgkhgrdp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gusssctf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2maylthbd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2koipwpvg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rpcniobk.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sfiwhpxq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xzuzpzha.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fvwdbgtv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tzmmqvzk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fddftfno.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kixujheo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sjaushma.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zbyeruni.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2bsiikbdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2suoshvrb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2oygdxzlj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mqbfhups.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ovrtrita.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ixjcfslm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fpdajyyy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tzunipqu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vqwffzfn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2qxoggqrc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2lopblkhz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2gihhzqmt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tptpbhhw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2fgzlajro.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2hpjjeifq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yrbbkrua.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rddautja.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rinuxhjk.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2svgzmuti.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zadbcfip.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sykjspfj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pmkcclsm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ecrmmtoo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2rctnkxmr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lpexxeqk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bisqrfxu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yzoghkwk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qvnwqpyl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2axzzvyjy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ogojkefc.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2clwqkiyp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2sanwgaol.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xqcdvzww.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tqcowxvb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sumtjxrt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xozuwyhz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lowgevoz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jjodzjfl.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pzlaafxc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2leuchojk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ctyaqrpy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2scrlrzgc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2agsjjudk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bugzpeho.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2alxsfcco.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xrurckem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ltkygqux.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oxetodqh.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bweysdvr.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rxwbncho.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmphvg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2cxthtpqf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xspnewwo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uqsimxav.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ztrvirrx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nzshucsr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kpchqgkr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2disrjwhq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2btsiuhme.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2qycypnap.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2blxswhtd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ppymiqyz.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hxuoscuv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2xjxtvwfx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vcceuafv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2gxvevqjt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jjrxijix.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qtkitmji.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rvpiilas.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2nynpjtqi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bmirjegy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pekkayci.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2waufngxp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dkrejcue.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ymfcwhzn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jqspewnv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2yyudsnzc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyeznsua.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pykuxsyt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cynvcbfn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2esgtkxxq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2rcshadaj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gpujtxyd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ppzvpcii.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qmyqqojg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2qgvcubdh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uxnvylvt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hkdimzqj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lxyfvraw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ylhtyozx.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cwtfmysj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vleozfgt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kfvtaywj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2anvfnzhs.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2voukjnmp.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vyrtduqu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnigjdxj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2labenxnj.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zeeskdkp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2upqosnst.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fvgngjko.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2otnybrbs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gbhrsxuk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lhdyegpr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2bdgtvuej.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fgqwpqgf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2iphjgrfi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qafzfziz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2czvzkohe.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2voickubb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2odrlkqvo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tnqvqudt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aocpgrba.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2qetditph.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dhxcrvjj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2knlbvqze.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2degycexi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fbzuuvan.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ostfiwft.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2cuapxseh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nimzprsn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2apxcblhd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ogiidkfp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iopktgoz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tucstarm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppczjmkc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzbrkws.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2znatgldk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2atjwprii.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jknawzta.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zhtmkwpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxbnvpsk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjkruxac.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sfoawaie.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yaxxceis.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mipacene.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mumxukfh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qfbqzsol.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wolveghv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2cwzdhwai.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zkkuscao.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ukazabnb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qlwyughk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xhhzyniv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2rlmwqwuq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2gkfkxcns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mzpqqsou.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mkfipsei.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uvjvbpok.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jbrlokue.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvyegii.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lzrexdps.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2spupsduu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uyhfetni.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gejnbecj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gtufipzt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2wwdllzpl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2cebegdic.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tuxganlo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zjlqhveo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmvdhzr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qonvjcxq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zmzqesjw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkmaookx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfyeqxhu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dsasyedv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2wgakxtgp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fjbtmcyy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hiagpukd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eomdjdid.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wshxvmxe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nsbyqdgr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqjdfauh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wolpyvqv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cfctonwc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kewfuftn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2sqpmverg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2moxxvndr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmanucfv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mbbkusvy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qbolxxkd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkgudqvj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fxbsybpc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dxomjzhl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hqefbexb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fxkfvoec.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eykppnxu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iehtkzjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2czexaprc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2syudowld.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2aozapffd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bjxnzwmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2grzvxhrr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mvcideex.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjeykjwu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2eqwgqmri.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2halfwwhq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hlphmyvo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ovxarnqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2srzclitc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfkfelrq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jfnfdeka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xvmipzee.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mfxmhvdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdmnwgph.html


<!-- 参考信息 -->