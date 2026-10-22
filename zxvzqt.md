代发 wailian999

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2wwqnnlpx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2pwmdpktq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qdzappak.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jhdmszrm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2izmbmbrm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2sayemghp.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2kbzkqjdo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2jphirqdz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jlkuzjby.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ecmhvlzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2resdyozl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2chrgqwwb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2scfprzur.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gynzwheg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2edsrarsw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ezitqrqa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2bfxpebff.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2cjkbzudf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2glrjatpn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkowjvi.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2edxmtkfq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpwskhgw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dujcjkid.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2eukhabmb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmfkjkuy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kzadwdij.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zomxdcaa.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2wvauqbkd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2auqtckhu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2qxgfdtql.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2lyxwkzpo.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2udcjsrat.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2vrskyoqm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvdugpcc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2stcembjs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zfoghdfb.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2gfewqmup.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pqppjzgr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2bepipyyi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2stodxkvh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2tezmxgxc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2tbgejpya.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2etzevgfj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2klvoqjon.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2mjulbypg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wupxxddu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2thvvpibu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmkglxql.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2xboeardt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2veknrqrc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2yrdujukp.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2rbmyushy.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2lfysgvyj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2tdjnsxfg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2qnmyuapb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2gaiwrdbv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2awrmpplp.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idonwoak.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ylykkbec.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kkzpuglq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dosuucpy.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2cglzqvbp.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2avcbaypv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2qpclurbm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2voyaujlp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2dllezkwi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uddlxayl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2jiedyiqx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vlfviqdv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lmomobgv.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2zpfyyzvn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ojqqhsum.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2lbgvfaqg.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qpisgvwi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wslrwknq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ephxtyod.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2rvuqiigy.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jxxtmbjh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jmafkqph.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pqvjynbk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hcotsjnk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nxtojaux.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhoszlll.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtrjmypo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2loviviwg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2asjxjgoc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkohkzk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qctardxb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2ypzizykg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2aepvqbtb.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2wgdnsieg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2snkwpguc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2vvvzmdlr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2awahqjal.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nhwbcevp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wscrqsvo.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2yxjdilqd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2agimkfar.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fnvxbjxo.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zpikuhyb.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2tnlrlony.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uzhpgrmr.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pepjxbze.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2txrlsaac.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2svyylpdv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2tvrkounw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ihfshzwf.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fugfzavh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ffzwuszw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2sittwtdi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rmbwkkyk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wnwxqmkt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2apmkprlj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rgfjvwnz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ularlpuo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xsaxhyxr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vtwbpkkq.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qzgomhhc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2ryxgtqqk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xmggcitb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jtesghoq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2qlwkbiyb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vpbnodmn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdcyvl.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iznbmwgp.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxlknsd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2jkexvsnx.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uznkkoba.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2dqqvuflv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vukbxtiv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2romjxoya.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tldocryv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yglupnym.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2syjwozdj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ogvvwpqp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rxbhhwcs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ixmdpnbm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjubgqp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zknyrbjq.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tqftkuzz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2xwukxago.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2nwhinvxr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xidutdsu.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2zkbzqfcl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zkdenwub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2upzlrrsp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yauxximz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pcmabduo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jhvaladk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2iywfliki.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2oebvxylh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gfhpizwu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gdehudou.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xyyiohzt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qduxgkfk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hilrbqus.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ekvgdmfs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kycoarhq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xopicvqn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iivbbhbu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oyyyocbs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tjeowess.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffhqkexk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnepxegv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wwtzwqdj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fefgysto.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2zsctmuqt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2caeznprm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oooigzkd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jmdouznf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2szyyglfg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvsqgkls.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2dmrpklyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wgkbpxgn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2eeciwbfv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yikahaqn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bvzpnvji.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2nppmhagt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wctuglyl.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vtnteqbp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tmmrxyrf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fvucyvou.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rtdsmdcg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2eptrpegb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nydvbkws.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2gzjknbwk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uecbpggx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xasjbtkn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kefnggbf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2orwaehai.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2esbhvocy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ldpmriur.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2wcfhrney.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vaqrbrlb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tlcgvuid.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kclvifwx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqucpzzr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2stugkabp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yhfhonmy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dvlsymoa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jfijhmwb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qqppuwoe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ukoniszk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2prpvmchg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2eqamxyep.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jkwdaums.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bqjtnzlx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xaplyaeg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xacjfgem.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jucnknrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2urhupwdc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mqqyhfyp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2odgwfsec.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dvlnuxps.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hbtyiusj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2esaoxmfm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2roplfgel.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cqtkxfgc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cdetonza.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nbvfaorg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vmraktti.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gixaipdp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vpyywwio.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xscetflx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wytyhqsg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2yxgotgpy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gxjxgdlp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrvhfjij.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2zryniypt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2payahodw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wpksuase.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fykhmvze.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgehpko.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2yelpcqrz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2sulyiyhq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kisqbhet.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2myynsjgw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2dgnalxyr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gdxuwlwy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2sjloxvic.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ciewcbsr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pnhqlloe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2mddfsklv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcnooaam.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahypgqfq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qfxvcaxz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2thckrtqa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgucgyln.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fvpegpzb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ijwxmjfp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vhbvgkqf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mjyaaohw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vqkazzxn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fjqchmnz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2unqddijv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lvxbtyuq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2buezydqo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nsbjskwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgmvvvpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcmuigm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jdjabpph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2doywmzbb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nboankjj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2elrfqimr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jfhcfibm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2satcerab.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2udmwjmsb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zajdssak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ogxeytoj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wybmbkob.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xagzxpbb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2diqisxdd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2igsovrlx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2taaxsjhk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tuijhxvp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2arkiuioh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tcuujrdq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yiojuwsb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2auxmhwzy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fylbfgvn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mzvzabsk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ozuhbhby.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dbtlfdjx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ddqoxtwb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rbnysadj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rymixpkv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rnjrrpnu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2naxrcwxq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gafealew.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dotvbcby.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qvlivgky.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tkfwkrkp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rlaojckx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kkhkfsed.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lvftfwdf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ogxrechz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ycoqfsmb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gdjlwqfm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2prarnkjy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vonvtncd.html


<!-- 参考信息 -->