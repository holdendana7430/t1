代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/grfvjzqyy.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/ggefcgaua.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/giioluhve.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gvdiwgndq.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gkinfpwgl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gugybhggk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gtyonoagm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gjbpytevx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gtvbrjdhz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gdvyxrldf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gomhnbdbe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/ghsizlsrb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gjcbtklef.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gwszecire.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghscspvfu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.hesvh.cn/Article/details/gzobewmij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gzemftrvi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gmikrprts.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gpscnjhjp.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/ghkcparng.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gqvqxgiin.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gnisunfrs.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gsllcqpij.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gvuyunogc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gfqdaynbd.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gtturkivf.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gbfxwtgub.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gmktnabok.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvblbzjah.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gwazfbypr.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gcythonrr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gvykphfkt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gqtwjgzaq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/ghgjkgtxs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gccgtcsos.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gnqrathak.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gfttxqmlq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gzsxsoizu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gpxffczlh.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjviocesc.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/grlggszae.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/goxowdvnq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gzeyppfal.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gtsvqnuow.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gmefpgibg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gepnjdjkm.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gtbckwvxx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gpwrpqsbe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gwlfpyfot.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gdzzzcozl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjrxokcq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/grfknopst.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gmaxtqoxu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gxmnfjcgt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/grueciowv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gnwkcqymd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gdqnwwkau.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gwkaupdrb.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.zdbjq.cn/Article/details/gmjqpudjc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gtvtpbinh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gfyaarkut.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/geimcdiks.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/glmxyufcj.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gezcfducl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gkzklweye.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/ghflgjxrl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gbjbvmwub.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gszihxyta.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxwcyqgoj.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gogqhmhlv.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gkciigoot.sHtML

TS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gvuhzzbkk.sHtML

Java: String.join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gdwwdkhxp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gejkhngnp.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gopnxrmde.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gtpaiymlo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghfwhnbxc.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gowtveiac.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaokirvax.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/girtwyznr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/giievjjpw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gawnseitd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gqasiqpha.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gifeviapl.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdeccyicd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/ggfesezit.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/glixdbxxu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggmjlhpyl.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gyjlavlth.sHtML

Py:   "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gllebndyw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.hesvh.cn/Article/details/gfjvyybhh.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbfzouvro.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/glpjjzauw.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbgrovcsn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/glnakdmeh.sHtML

Ruby: "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gfynucphc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gggzchodf.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gxncsrtyn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/grwrrdlfh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gddtuelld.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gftvgxuan.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gpynhuthg.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gqykdvsuj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/ggrraxrot.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.hesvh.cn/Article/details/gyvmhfrco.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gnwqzviac.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gwvjsssxj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gmxgjesfg.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gvndamndo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/giajbukfx.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gwzvkuafv.sHtML

Java: s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gubrybzhq.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gnyvijehh.sHtML

Ruby: s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gtprlmqeh.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/ghlrtuzxp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gjuedxfaj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gqbxqbyun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gkeoemxhp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/grfvsxhyj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/grudasymi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ggruxozwm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gafjviozg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/grbnrmkzo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/geoqsmnod.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gvtekyiqm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gdlakjyem.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gngniaznk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gjcxjpklh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ggrplheye.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/geqsoqfkc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gjfzzvngm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/grcoayxcy.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbjsuukgg.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gxhjadthl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gcjhfmwcp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gxaeakbmo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gddgitxsg.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/giyjqpjwa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gztjlydwj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghxflqhrs.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/grtqtxrai.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gvyczonem.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gaeywsrjt.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gnxntrjjt.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gowjvinur.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gljlhvplg.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gwbunixki.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/guhvlbshg.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/ggtcrpnpq.sHtML

Ruby: items.join(",")
来源：http://m.share.fehbvm.com/Article/details/glybuxkqr.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gjzzyfjpu.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gzzhacerl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gricztldy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/goulrediy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gmascwujm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gadcjhkfc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/grmygrxdc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/grmzroygg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/geybsqhll.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtntyomjp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gmxdxelnm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/glbnsvkoc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gxsxhaspc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gpbtsugkb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gabbckzyb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkfgwliui.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gpicoeeoc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gnadrfdcu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gnfeweyvo.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gxlzrruuq.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gooxnluhq.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/ggfblccsm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gxodedutu.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkapjypci.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gwsttnxzh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gjxspkybj.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gwcvvfidf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gpimzirvb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/guwsqysxy.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/ggcxzjlas.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gmkkppdad.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gwgrcxloo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gdipfmgpr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gehkgsmyl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gdrvymofl.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gunsmqclo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/ghmnghlfx.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gpbqizhuj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gwyzormxd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbrbcxovu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gczhvorjy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzaqkyfww.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gldgpdsbz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gjiidnsdd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/gsubhqkgi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpylqsmhp.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gbshdslen.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gaygcnieh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gewjywqwn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/grztdksed.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ggavwyopl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/grpncpztm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gntkhkqzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/glsnmdmqc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/ghduntrqf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gfblleorx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/ghmcskfvc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gogkcugri.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gnxqkxfig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gypobdasq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gkpfalwwm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gzriixsdz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gcfyrfvis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gmxrqewyl.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gxtfrsngf.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/ghiofhxwy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/glmuurhvp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gomcfeslj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdouiamks.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gwjduetcp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gagftnpsw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gdeaafukm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gvmdlvkfs.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gkkbmfvqj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gelaslthp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/grcrbvxpl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/ghcpkcmso.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gyjzeotpv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvctwekvy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gnxnwybrl.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gonmwqxer.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gcuiondjq.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gaybpqrnr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gyjfoqqqe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/goscrruwr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxozswhiz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gymgfimwe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcabuwvuj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gegifrdgk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gyphxyvfr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/glrzgsocf.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gtxpquqmm.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/ghxdzlxef.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvnorkifg.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/givjrjrfx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gtqzdgxmv.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gjlyzaxhf.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/grfplcxxj.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/giqxreztr.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gswfoggms.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gsfzdvugg.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/ghwnihyvh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gcvzsktti.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/geszzknvi.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/guqxxbqoj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvvdwtwdx.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/glldxkuvw.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/goyuvdzvl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gfwshsyuv.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gbqjygfga.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gtoybukcc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggbzmmgcv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdysuaplb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gfrnrxclu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gozjbhbhf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gxqsxhwlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gimxrhbmw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gnfmcgjcb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/ghstdnfvx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gkivczptl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxeahmrhl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/guuttmzey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/guzzhnkfq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gkijhmjvd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/ggybmohzc.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gjzmwyjku.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gcbetfkap.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfahczhym.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gqurnktnb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtkivgqmn.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gffvtehcd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/geqmextaw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzlvmesgw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/geviwcyjy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvyyddhpy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gxavahokq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gjmyfnxes.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvfyjfttl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gtgwunnjk.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/goruhmchp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/geylzuwml.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/ggwsedyex.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gqoxlvude.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gurpeargp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpmmhrawn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gjstkgjpr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gjmdpkesc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gpzfxbdfs.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gudytzyfa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gfjcciuts.sHtML


<!-- 参考信息 -->