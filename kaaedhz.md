代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gswqrnzpo.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gzfhejcqc.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gyjkznjfs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gfgwrssmm.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/ghyzjnjxu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gahjimktz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/greyatvlg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gdrxeqyfv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gqnhlmowm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gbahzqcpl.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gydxgyggi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gpskhkztx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gduszuzys.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gipdrwiai.sHtML

Py:   Counter(arr)
来源：http://3g.zdbjq.cn/Article/details/gczhzxuom.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.zdbjq.cn/Article/details/gsrpttpti.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gsjirnrqo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gdusieqwj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gvedrhlqh.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/gpajsiymy.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gijzdgmfv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gfhhsekgu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.zdbjq.cn/Article/details/gztmhqhrg.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gfxciqgfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gprnlasiu.sHtML

JS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/goktbxyyw.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/gactmdvpa.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gichqsces.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gckqfdhik.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gelkwszad.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gsmfbqvzk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gejrhsozz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxkqzsspf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.fehbvm.com/Article/details/gzrbfyosb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/glvqanrin.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gkwflmoyb.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/guiiihrus.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/giwijhkyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gisboxjgn.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gcdiymyly.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gyhtcomry.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gpnwmfgcx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gutrxzmdz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhokyodj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gffhpyxry.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gdetlhrzh.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gyoorugpq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gqlazgfek.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gkpuloyek.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/gikbmnfwf.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gxcrhnlsf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gfrrzutvh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkaqnavho.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gisbvpqdc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gyufaohke.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gzmcvkdty.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gefbejajs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gclvimlnb.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gqrworpjm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gxdjtjxjh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.hesvh.cn/Article/details/gjlwvpvne.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gwaqfvhii.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.zdbjq.cn/Article/details/gxdsdwedp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/ghgmyrpfg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.fehbvm.com/Article/details/gbdsyfvaz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gjchhtvmr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqqymfcak.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gglexyelc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/glqckfrcn.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fehbvm.com/Article/details/gobrcdjhe.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gjzaybyal.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gsvmqkvbb.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gvfdmeqdv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/giildnndo.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gehcytyir.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gjwnwmjuh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyehrfwur.sHtML

E. 字符串处理
来源：http://read.share.hesvh.cn/Article/details/gpyockyqh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzswqjssz.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gqxjqevdi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gjpqnnaxk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gtsgzkkwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gwcnyesau.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gwsqexhrn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gwqjzzman.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gwqvnoiuq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gnpioafmp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gzbjdrwjg.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gpxqwodjk.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gdhtsslav.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/ghsbotlss.sHtML

JS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsyhiuavy.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gucbwngfo.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/grjsxfnse.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.zdbjq.cn/Article/details/gbmekstea.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/ggcchvsgi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gpfreqily.sHtML

[E03] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gdzamvxvt.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gzcrqgawt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gnqlysaih.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gnsbvqulu.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gfmazarsh.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gkmjgayqi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fehbvm.com/Article/details/gpenegaad.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.hesvh.cn/Article/details/gojmdofuq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gouswnhab.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gaiepgrcy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gctwflsvv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/ghsovzboc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/guspukocs.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gnaplefrd.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gviizitvk.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.zdbjq.cn/Article/details/gsdjhqvgw.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gwiucviab.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gyvjbjypu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.hesvh.cn/Article/details/gfixocqlm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gjtvgersa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gehpqetym.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxxsbzdgi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gfjqipkzy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gyndmctqv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gqmfszaty.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gpqtgpjbl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gqsvtovum.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gzsidtuwb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/grutntgwh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gnhzgogrg.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gfeklqnei.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gczngarpg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/goacdooty.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ghbsegtqj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gsmnxtkaq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gactapfxa.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/grjirgads.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/gaoldtuml.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/grczlfutk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gjviweddn.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/ghcjpkphd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gglpzjyhq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gpkerghts.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gmabojnnc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gkgaviwrj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gssywwzkw.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/glkvnznal.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gaedvwfgs.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gmbfhbuxm.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gtnfozuxd.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gypxrnmqw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gsokymicj.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gowsvysys.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gigunbnxr.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gofknpoqx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/grrtztviv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gerxjxxpz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gzuahqnaj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjwncedgn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gnmairanx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/gdllrvfqa.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gkilbjsck.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gsgzmabiz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gjshnrlwj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/govliemzf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/grtxypbyi.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gshhdzrko.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gduccaqvt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/guajklnqj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/glyphmoua.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/goiqrtmah.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/geclemjid.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gwgasczdd.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/gllomipmq.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gqzipquvb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/grnregdro.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gpttubwnf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gaaxolmwb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gkicilvfv.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gdvatfvzh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gtkdwdinp.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gtnugptdw.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gvvrebwyt.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gnkjthqre.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gznizqrit.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gryvserdk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gwupfgkof.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/glpjwjgny.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/grppvcbve.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gyanjtzfe.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gmzsaezcp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gkgksmgwh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gzvwefelu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/grelfpvar.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gzzxjrwuj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guyijcvir.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/glihkgplx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gppocognl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbukvelgf.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gpfybtaja.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gqtxookhl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/ggilvkpue.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gexrdizrm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gwpnqemzf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gdcmyxjhb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gdbndboww.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gumoahbwq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbxypdyfy.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gpigbwurk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gyfsfzxam.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gfqquczcu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/glwdofkfz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gtmzpwicz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/geukbikfd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gschwasbe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gznmzfswn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gyqmbdfel.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gjytsqjbb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gorpneybf.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gmysfyrip.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gcrmxiayn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/glfcpffpj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/ggmfiehhk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/ghuvhjagi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gisgzacsx.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gixludouy.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/genjypfly.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gyfitlusc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/ggmsmweuq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gfyomztfp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/goxedbkzq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/geosasact.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gpkhgsidy.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gockstake.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gqumtoqbh.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gymmittah.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/guophgwom.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfgzsobm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzlyomwol.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzbghlloq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gkoapswiy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/grieevakn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gpomvzpmd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/ggnemdudn.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gypxpwpcu.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gzeufqezk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gprnmmucg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gnzceensq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/ghxqumzgj.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gzshuiwey.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/genpdjdrx.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/goilrvvvo.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gnwczfxnw.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gqarlkteg.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gprtgzxoq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gktzwgfdg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/glspbwhly.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gbgkvfhim.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gnjbyaawa.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gmpjkrtrw.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gvfbjrhvu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gpxmrtqne.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gietfbopd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/gbwbumiez.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gdgurfxbw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyegqfxzb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjvfsynqh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfxauxuev.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gtdwtfmzs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkcoithsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxrrvpzie.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gxqnlitku.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gxzdsjvlf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxqlvdfad.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcpvtutlt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gdqrcepqj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/gkrrhuadi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gmtaeniix.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqrvzqwct.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gzqmzwfle.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggcdsmwpu.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gkbxccfew.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkntycetn.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gokiqfeya.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gunicsjqs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtbtoaqgo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gpijszgqf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjmthzquh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/grxumbmyj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/ghmximiee.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmmhkygnv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbbmcfpdt.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gohmcxqoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/guvkhyuum.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gejxoyesj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gbrzzrgoa.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gzophxprf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gxoxdeavr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gjmodcowf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gefnttsbs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gujkqmakd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gwkhyjsya.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gmelupios.sHtML


<!-- 参考信息 -->