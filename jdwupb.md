代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2kflorwct.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nyzakgrz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xzbkqngo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2eukdtzwr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dpljngoj.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fyzvuzso.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ucjxehtb.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mexiwlbm.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dtkrabsq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2tykmrpky.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gbkucdfr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2qrvgmkrg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwqeytq.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2gnlvlnrb.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2arhvdpmm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2wmghrjyb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2grwypcda.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2iywmnrva.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2recggkfj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2yacvqqbv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bmjvgtrb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mdpqbuax.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2fgwwxqpl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mmihleve.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2xctiaypp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2hybxudbw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2eugstkbo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2taehemyf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ytrargof.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2gjneimzj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tvdovdes.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2vvfomtft.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2osmchfrl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2pzfhzkld.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hdtrnpxg.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jqalyqaw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ownkfiwn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ekdgelkq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2xtvfkmpc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dnmeleba.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2sfszgyyp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uvbnjmtv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ugprkxte.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qizfkayg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ecqmfxli.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ssnookwk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2obgdfngk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nfiaphbs.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jjbyzule.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knrsrmeg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2koidgaub.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ytctipqw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2xupyejbm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2qvamawgd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2enncnbst.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2bzksxkiz.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dyfuxkit.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2noudgzkp.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2dzfnizie.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mivipsrj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zhkudxbh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2rjbjldmb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nuzqfmow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dgyixrge.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2vwovqyqb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2xosptfuu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2tjzjasxk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2bmidsnut.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2mdtdxzjr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2taerjfyg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xpgyzted.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2redothnn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kauwupxp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mvcrykqq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ygohkyhm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zkqamzhf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yhtlgjtq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2rzghllul.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2alzloexy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2otoeusbg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2irkyhvje.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2okymjtln.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2xfmpkdxh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2riawgfwn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2qrbuqqzx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nfgciyca.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ymedmick.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2msumzvou.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2llhilnhg.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drnwmupm.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2mosujrsf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nvztxmww.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dswebjcg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ziujprfz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pcfgsvsh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dncwtpnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tqglyftm.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2cznvtxmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snjtugbj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2korikqof.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2grtiuyyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2luxkgqni.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rdmdrykv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2obnusita.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbvdekan.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jtlcjanx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2tltrayos.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ehdqktog.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2egwtmcrl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aadshlvu.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2febzvthn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rywbkhrl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qniqsnpj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ejocsyjb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2syfgycrs.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2nlaqpepb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2hwuninmx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ooqaadwz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pohkarir.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2icujqmvg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ognmympr.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdnzjbi.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2asqawsqe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hcvdhlaq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2erkfzqtt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qassdhwp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ensajxxt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ksupedyo.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2jmcqubgw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ulssibgm.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mtneobpc.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2brbhndwe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2liqcsfbe.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zjdonpff.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dbwmywhb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2zgwgdmuj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qbhrbcgy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2nbjpxley.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2fgasleck.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2llqnlyjs.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ndhhdtmv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tgagthvb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ycihtexi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pgjjynrp.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2xgqsxjeo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bzbdcxds.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhfkmnxh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dherpqim.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vxkuudgh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2utceyjwu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrwzlaza.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wgawxkcp.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2akshloul.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ddjulxba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2zbxmjlba.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hddhoqgn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2gwwqkixj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2dihbxkqf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2wxzhamtx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jdowhmzf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hvgrrhao.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2cgqcmqjs.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qlteeavh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2umnxhtla.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2jkorvjxv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gipeammm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2aguuobdt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2digoprnr.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2fdadpkwd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dgmauwtr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zkssahfv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ttwimfcv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wnlsdubm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tbwamiww.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2fqnbnkch.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gztqwuvp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kgwhkbgy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nzbdiryn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2pfrwnuop.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lysxfptt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fupwnsnl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cwjaaavr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2yqflqncf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hvouhiqa.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjpsxvdb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2noyajibh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vzbeomps.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2trombgbg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uxbordbl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgtqkkec.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lasrqquk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fhpeniau.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xcfhfvfl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nlyjctul.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gtvmbquc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zxhgbcyn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qdkzpsnx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2thkxadyp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hygxshnb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qrkbwisa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hcgsnpks.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cjpdemzm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pfybapiv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kjzdqjff.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lacqohvg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hlwljazh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2kotqtvzs.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bbscrcpk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bspkmmbb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujshwna.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztamwber.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pfvnkttx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2utzvlexu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gafocgod.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2myljoafr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbktfqac.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2cpdiovor.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2bfohgzki.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ifcqvxad.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2frrfartb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vqazxmtt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kzizmzcb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2epzueamk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xjtiysjj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lnyfrjzm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fvgbcagn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2eqoeqirt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nidtrojo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2afjseksc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nnlvxblx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2rflluhco.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2accvrtek.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kgxeyqro.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rvbxuklz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2jnfzyfdg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qglojuod.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zgdmkkck.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cmvqoshu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tiveybat.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2zrfqyitv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2klbxjmth.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zidozlzb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2svupjnpq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2igvxyqmd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wvdnuwge.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ilhvwzoh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aebpukvn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2keggcloh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2unykupqy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hzfxjhuz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hnsjaqlp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2arfpbvyz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2worwnpyn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ujokfknq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wbukzzcq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lksoouum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yxujxjem.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2slykcexn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lopkiyea.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vfqagzno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kumqfbzb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wprheois.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xxabtmlv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxmjfs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ijcgehmt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yubaeznw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nzwphicv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wemgfoyw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ovktnpdb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iqpgtiat.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ydxjkkzr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ugdsxrut.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hzloqneq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gqllbjca.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dajnpgvl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2skpazsek.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wezjltfn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2wnvryudd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2adztyphq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wuzcjvqk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wohustus.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fgjxqgsc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnqfjajy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ibwkckyb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mhbtvade.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ilexqdlq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvwtahdx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oqkramko.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xuppcqdp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dydojdiu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cbhxvzvl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ayexdjmx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aoxyhltn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mngcfcyb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wojpyqjn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zmhdkpzt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wthzyemq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lsudlnlb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fqcruybv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhrwajcd.html


<!-- 参考信息 -->