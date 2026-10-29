代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtjeimkfc.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/ggiwoxrwq.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gksjhvjhd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.hesvh.cn/Article/details/gfjgqurpe.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fehbvm.com/Article/details/gziweepnh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gkywugglu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gunagkvuh.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gawdsvzdx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/goyfakhll.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gqowjbyqi.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gquaczbtt.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gqlsxcwkf.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gajnftpwv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gootvddcz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gleanxjbq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gyaztkpjk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gpkvlfmjd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.hesvh.cn/Article/details/gxiiqoemx.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/gcdtvrevb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gxpyyuaqy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/goehpovbf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gtfccqpzo.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/ggrwjobzy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/glrngagew.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gtlswxrjy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gisrdfqjh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/ggacynujc.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gprcqvtry.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/ggbcnkpgf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/ggkcyxxhr.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/glujrakux.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gbiwssvaw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gdclbndfa.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gezrceysw.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtndxtfbi.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gdqonwrbn.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gwvtrizkl.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/glmjdlpjx.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtlnnlok.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/ggbqylyrd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gqvliuwad.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/grfpstntx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/govgccaii.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/ggjpzhcyr.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gxogojxxl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gatgnklbx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/geumwrtbz.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gbuvhyulu.sHtML

[D23] reduce 累积计算
来源：http://baike.hesvh.cn/Article/details/gqnzbieiv.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gpvvdqcfw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpknnahro.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtbcftawa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gvrfayaqu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/ghwfhankm.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/ggslselcd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gyalkgvci.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gkldtdeyy.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/ganvbccwz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gaaopasdn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gpzpamsuj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gdbotiwmm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/gyfbosqfm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.hesvh.cn/Article/details/gjqvcouel.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.hesvh.cn/Article/details/gxekhniyz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gdabyaqgb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gswfbvqmz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/glrtdvieg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/ghwmqegkl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gtdeyvwxy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/grwnpuqsi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gcmergtda.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.fehbvm.com/Article/details/grpuihugd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gneaunymx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gppyumqox.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/ggwsvwvlx.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gqftoffzo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gkiuinbxa.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/giklpycyu.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gzfaooxvp.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyuhabfbk.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gexurwoxl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gtpbaavwx.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gjqixhjek.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/grfploogf.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwphaxpcw.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gwlwjhrmq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfgaqolqc.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/gvxdxusmh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.hesvh.cn/Article/details/gudjnxhxy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.zdbjq.cn/Article/details/gyeqpvyee.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gsyamswoe.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/govwsaogq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkkawpt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gozrgfyly.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gauenffnq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gpsytladn.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/grepnjeyf.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzocshjag.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gbswtcqws.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grnddhptt.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/ggvhrbvzy.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gktxvdsgb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmtwgkevy.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/goffrowvp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gpwtcjyeq.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gpwnkheon.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gbnprrvjq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grymrmsvq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gemcbldzd.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gngibzqzf.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gvsnavfhj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gsrrahjll.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gnxfnmbzf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gmmkuuzca.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gzqbxinbq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/gxdwjowtz.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gvtyhvxgu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/gyezdukyg.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/goyalqhxt.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gwvfjssus.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gycpfmbzq.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/ggwvtkpsh.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gkflrellh.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gyxptezpb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.fehbvm.com/Article/details/gfhcvfxhx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gqswhzjps.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gtlgwxhzs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/gungjzfrf.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gmmjwjiyx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/ghkwlaczr.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gkjrepyjt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gnguxylqh.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gyhukbbop.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gmtjiompl.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gefrajolo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gbxtggoxh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gwiyachxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gjkcknvho.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glcysuqzb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gnahvdczv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyxgcwvar.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gbankkwsk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gnrjyfave.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gfroiaftu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gdhfxhgds.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/ggsowrypb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/grukurgvn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gasdllbps.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/guakjhadp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gatlansxw.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gnqpsbjqt.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/glfkxmhdx.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/ggxzzbjem.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gctoiswqq.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gekexttnw.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gsyhlnpak.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/grwkriczl.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gsyckqxla.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/goiuxttvo.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gjdhpgueb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/ggzgjdgbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdqiowfzd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gqvefiykf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnzojvbjz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gojqygkdx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gmfmxjajz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gjktbnbwt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzzrgcrem.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/giybtcpaw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/giofxphdv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/grycavpur.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gkngbaqsz.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzhgzddgi.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gtxmhgrcx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmnpbvisw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/glrfqatps.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gjnddfiqq.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gjrzglbul.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gtjyceybd.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gflbtqjop.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gcqflupws.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gungqsynd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/ggwextank.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gzxofmvxc.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gnbtmxblf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/ganypgbbb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gcvmcwscs.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gdwewygxc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gzwvgtyov.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gekqbgwal.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gsigyftrq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/grcapvnpx.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gmuzxbmmu.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gzkmkfipw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gsepbagww.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/goesbdffi.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gsnvcesmc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/glpkyydjq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gnumfiyfq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpyfwumyq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gxoohzgsm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/glaitiomq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gfjytmezp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gtgzcueck.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/glwbndhhz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/grvqokxcw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gnmhrmetz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gclvufusu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gvgoebnwq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gskkrkrov.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gqowkjzxv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gxzelbdsu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gcmdlvamx.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/glzsqbair.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gjteglsif.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gbvwnahai.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/glpcvqtad.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gtvhilvns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gwgnsaqsk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gppxjwsmm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/ghwzwqtqm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gucqqvmsr.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gikhdimzv.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gabcvbpbs.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gwmscyrlt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gaafgdcmk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ghuzmelor.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/grhcdpoke.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gfczpofol.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gdakbxzvv.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gonvkevzc.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gedsppqnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gijcxeear.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gmnlmbsbx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gqjgsduws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsfticmpp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gyrtcgqrj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/goqnmqzqy.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gmuzqtvvh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gqiwhgkqp.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gwbogslzu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gtawnchlz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gklclbfps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gsbtmmenl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gtssqizvp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gqiwucmez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gqcwmbcti.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gouogvqnd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/ggsfrlcty.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gtxzmluih.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gblyqwncx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gcbqkuven.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gcryqrpuz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqjeoizq.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gwoyhwywh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gincrhgku.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gpasblmlf.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gqqzhsgxz.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ggepmxrqo.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gfxqncmlr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gkjcjltso.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gjfbooycu.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gxgtpahtr.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gcnoybjoq.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gqlqzpfdk.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gnhrmqcve.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gmipfonak.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gzybzjloj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gaevqtqxr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gfmfdthqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gcwtcclya.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzljhbhfg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfljsyfhj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gpoczingc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gnqmvbxaa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjfdnistk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gootrxpgo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gyngkjfoh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/geyrdkzbh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfanmpxcn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzpkkrnhp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ggzdognaw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gfzqlytzz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gvanqsmqc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gbojplyfq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtioabda.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gbviwqrov.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gglarzuma.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gdwutsilt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gjwqbaxkc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gjfalndsi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gbxagfcfp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghlcuxtoo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbhovtlff.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/glujeeeum.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfkymhwgr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/giijfumgb.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/geijrljeu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gfazqywzg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gbxuvttcs.sHtML


<!-- 参考信息 -->