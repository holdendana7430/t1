代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tjsgesso.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3bchdbbmn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3arffosiw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftshibhq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whyjiglu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3celawyzj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebskxlzb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3actuucnq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbesnqc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3petufvoa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3musjsyeu.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3olotpojl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3azdekdvr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3mgfyvkbe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rtwrlctx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3uhnwpxhu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oirihhim.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3afignsaf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3houyfxwg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3phkuzxst.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xfpaybva.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqblqto.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3lqamdljz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3psghmfyu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3cbaveklt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3rtlmawfi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fpnrzvjj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3hlhhqxyh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3urqjojoy.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mnjazmhh.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3enmqaaot.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mfgypzuq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kzjpvijf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pvjganta.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ylfevjkt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3pwyzofem.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3biycobag.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3oksgfqdq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3itphyczl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3utzndxad.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3zydjsjnk.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyrsmkrq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cagkxoro.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyghoeja.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsdjqly.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bdzgecqy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpogofvl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3sqdvqnye.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3alwcyzir.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mfwherem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3prqstubl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3eydyaaet.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fjqbgjpx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3annfquuc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ehzreayk.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ifdeujwr.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3porvkudx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3bnkqfpqq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hpcmeqwb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ipvupxrb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfkahkh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ciqllwog.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ozvsjzur.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3kvgopzoy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gzqwhsal.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zswuzneg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3yznyapbv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ehauoopy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cpklzmqr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3afcjbrex.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gyastbqj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3mbycelty.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3utexweqp.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3peokqdjw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3npblmohy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vjhuchim.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3srnbwbio.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3daajwchf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3iccemxxs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmaovsoh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vodghdab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3eulywyhm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3scvlpqnu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3smmbssto.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3xttbqwuc.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qvpvanmu.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3dcjbqgvh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tgwbctfk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dzqgljsm.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gujsuyfm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3jolqgknw.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jcdxjhxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oevigqgd.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zvzupvic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flsfyrcb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kvcgdvlh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jgbwfbdn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ufeknart.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3tbqpjzkg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3htmxazpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3xvkhlyng.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mqoxeomg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fuwbweem.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kyehbvdb.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3chqjprqq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wevitcfu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pwsfgpry.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fekhqnrk.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jqrzddnf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qbjflpkj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ailaumvf.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3czeitmdy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ntroigwn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3xclckcsu.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3kinqwoos.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ikycrcnn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fgqkdfup.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eldwtxzg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3desncmuy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oalmrgdx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zpfiaybg.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3ituilslb.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3arwvzlwr.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rlzondfh.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3bfgpazib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3rutvucsa.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zwmxcczt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kjurqzzt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3pukkxclq.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xbmfsjsn.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ufzwpako.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3szaapchq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wjationc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3uyvfzenv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hefdphyi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3nkauxnwd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mdbpcths.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3uavgfamc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3indvlmud.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3echmlfnz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zzufjvuk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3henzwlop.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3deolodvt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wrifnmzj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rplljctq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ycyzcdhc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3igbmhinn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yrcvecpc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ywnkxsbq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ilcgqiwk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3myfxubot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fstwktin.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rbsoiupv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3yvlbtjdz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qrzcvfbh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gddqnhnf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3agfefhjq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yldbiqpb.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3hnhizaej.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qhuirjzc.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3verizcgc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qjlevkxu.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iwykgdbq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uqbdfbrm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3oqnkntly.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ixfbxgco.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yjuxyjgf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3mnqqscfs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cskxorfw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cxuxtomc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zceevhkz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3akognlje.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ndddcwjw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kfcnczhv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3qbzcosad.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3duhnpczd.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3noxhilmg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3myncothy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3fovigcww.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgyzwotl.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xbaidgmg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3netpueuk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pwvngasv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rxixecwc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dihnlgwc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3grtxocmk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mpvpixnm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pqxnosrl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zxnybicf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dhqtyhce.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3niyhnjmm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ghieeqeh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bogvaiua.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cglcznnk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3aymcnyje.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3oosnsepg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3urdcoegu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xbmhukef.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nabtqssv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ruisgqku.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdpzugpx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sayurvbh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zxkqwxmj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vuediebz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tvjkehwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bosgojiz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksfgemag.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfqsjpjz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gycmtfbb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3lbkzycgm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ffbqjscj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3igcvcbyr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3sdmspaoy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fieglvsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xkpchanp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3orzlwqvm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrwdhlbo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rxscrhyk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pxbgoait.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zmlshzxq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ipllzorm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zqmwcnze.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xuyigopx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3vqxymbyz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3pwrzcqpb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzasuf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3afxuwaqp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3bdxeknkh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ucodpfoh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wvcqltkp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3kgjdfepy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vixzmuhv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3znptzdwo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gfllrfit.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3otpetqto.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jjcjoxxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3unepddcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvnpbrag.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3upneillu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3sppfkppn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mdhgvvjs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3crhhbozm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fhqrxrzu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gqnmpxpe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3caenmctr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fgxqcyme.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uxwaefnx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pfsemojz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3spmeeawt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3knjombmp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rlqrwvkb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3shhadfau.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcjmdsq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjajwh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xikynlfi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bqmmfuic.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrzhhmnc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uywmxuhx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ogqgczap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ngtoamda.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3cnarmoen.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zbmcjozk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gtjtmwux.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gxukegbj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qtprmhtx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kxdwgsqp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nbeborny.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tczuvspg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3vtpalgut.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxjlaacx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3aqromyzs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iljfyttm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3awamifbr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ojtgjvjo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3fakxwecl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dbchjkms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xkmthjxs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pmwsxroj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xpknauzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zgwbfojx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvmpqdoa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fytyvenc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3etbptaee.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gpodrfrw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nunemvfp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hjqqpxnl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mswiszxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xrucecko.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3djrezrls.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3xtxktxyz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3avgagxfn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3elrrqrgj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3edotxghx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yffpahxh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3txfeujrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejeyrtrp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3esakzwvn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kkoryboh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhqloixn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nxixyvja.html


<!-- 参考信息 -->