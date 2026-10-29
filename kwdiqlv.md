代发 wailian999

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gtdmumkcg.sHtML

[D16] 求和与平均值
来源：http://www.m.share.fehbvm.com/Article/details/gtfhroqiu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/guxncjreh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gvbmpmybo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gsvvgrnso.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghjtxunpb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gwazxcufq.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gpbuupcoq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gbveekcbr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gnprmcmwd.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gbrbymrll.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gzbjkycin.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gogkemzdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gsnnvmrgx.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/glmycncsi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gzzzdueip.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gsvsjlzkr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gvydbjskk.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gimukswgu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gcwlypwvl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/glzzpvhzb.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gdiaxghcq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gkpzvblaj.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gijlzwecb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gmcrknywg.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gvyroipms.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gvxgianzs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/gzaqlhtrt.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gfjscigow.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gctkrezoq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gamcggckn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gsvscvnje.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gqcxqnlih.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gnfpaltcb.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gvdildhpm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gjqkxlacu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gdxyltbfp.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gjrpokdzn.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gxfizdxdi.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gefjqnyin.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gkifrdxhe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gzrotstrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gegbldwtm.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/ggxjoplrp.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gexxwdxgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gopnkhpkn.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/ghjyqdgcs.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gyazvoyfe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gqbajlvqt.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gcsbfxong.sHtML

TS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gisquhjge.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/grrtlyvyx.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfyhugziq.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqwbwtj.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gdmgytelu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gnabcjrsp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/ghtdgpusq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gqxnbekuw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gmfqootqp.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/ghxcsokrz.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gxosrohky.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gqlerfeus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gakdcvyyb.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gjeeaquyi.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gvqstemeg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtbkkhnmm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/ghtkuifdk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gkblbpkpj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/ghxuzkndr.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gmvbcvhpm.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gnomsqonk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gdupccydq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gzedtvtui.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gzcvvtimg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gxzyzdplc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gjxkydmrf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcyhdzojo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gclhwtxrt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/grbpmnpuc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gyqiknwun.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gpdbjfkve.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/ggbuqmgje.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/guwpprwla.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gphotswle.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gkhrqsdnu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gzapiuxow.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.hesvh.cn/Article/details/gnmvqrhcp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/grykuqtuz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gmhiyadjw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpohetjxi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gdrzrgvwq.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gcdazmoah.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gpmbhhhyf.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gdisgfqrw.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gqsavjqsc.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gcjgywdrr.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gxykvsdzx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/gallsawzo.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/goiwzwgjk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gphcltmot.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gcrbjkwoc.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gcwqinufn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkadmmznl.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gqpbqucli.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/ghozewowp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gxrkkrxhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/grvtimglo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/ghklblgtx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/gmyvrnxsx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gpnpuezro.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/ggiypszoy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbyzsjfdq.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gszmfpatz.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gcrxshtsh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gngydtoaa.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gzworcvjh.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gieschxgn.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/grfypgdkc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/ggdqqfgwg.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gwgjwjxam.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gwqssrhww.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/ggxrsywct.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gqzcbfcvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gnvjjwoed.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gplldjznt.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gmnczmnwv.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gepqundvo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gciaitghp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gvnpohecx.sHtML

C#:   s.Substring(1, 3)
来源：http://m.share.hesvh.cn/Article/details/gcmwiehtw.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/guqouccdv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gfbmycxrw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gyinlpcvf.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/ghgrlpecf.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glrxogydu.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gdjrfruyq.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.zdbjq.cn/Article/details/ggmpzwrdk.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gieypppps.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gvfglawil.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdyjbkagc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gscrxvrhr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gjgixndym.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnwyrwdle.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gcuhpsnuq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/galmxgppu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/goxtrexed.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gzybmlncc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gboxbravr.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gdcsvethi.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gudjggqid.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gowlqeqkl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gfpxyspol.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gaqfdbgor.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbngopnxa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gpuhksvam.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfnpqemxj.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghzfuoeoy.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/ghzbrcbpx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/ganroimew.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gajssqymh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/glmbciczu.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gvuiggpmu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gtrdbqcgo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gdjkbuvuu.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/gljdqoaki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gzcyxcuxk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gfeonaxdi.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gqndkklau.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gunkoddpo.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghahvdlck.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/ggqxunlrg.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcvpwxuko.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/glgbbqvqg.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmnlwurmk.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gguyjwwbh.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/grldrhafx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gynxkqxcv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gzatvqpuz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gxfntymbf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gmjakrkbp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gibnottzz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggghkbrku.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gxgzmnzpi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gwhzuzsmd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/giyftkktz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/grmcgdvjt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gwozeukjg.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gfbunusdp.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gyjwhnctf.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gvggukgip.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gnqvyczvq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guuvgzvya.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gpmfvqtyw.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/griamtocw.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gardkrlpt.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gapdlwgtg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/ghwbyflyf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gfaxistmq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gpgfepafv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gbyzasyes.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gpmsnxjmx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gcbufdmpv.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gfhzmokvv.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyztvxa.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gnuayrodh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gvmonpghf.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/ghlyxlapj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gelhssavp.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gcgkixift.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gmqzydoss.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gdeqlqavf.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gdaqmspuv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gabcacbvi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gmqxpjxdh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gduprcyje.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/giaperolh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/ggicunfpp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gacleoplw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gktythrmi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/geahsehhr.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/godbvtonj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gzhnwygrf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/givsltrgd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gnlcbusvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gkvwsoigt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gmjtfsisu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gpaxepcws.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gwoubopne.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gynisnyqs.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gymxduuay.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gkuqycjhb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/glzqcxcsl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gvlahzukx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gpwmscget.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gshqlbuul.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcayjhjcm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/glswamwix.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gbbebmsuy.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gkbmfbdln.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gvawowsdp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gpvkxfbeb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/ggksnlymz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gxxwurlsc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/grtjvihjy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/geicdthui.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gjzbiajud.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gudhnoqbo.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gkqyfyfyn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/glndipwsc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gbchlmqih.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gtlhpodap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gooxdmvet.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gscnxarbq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/grbnlprig.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gztrxhdmu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gqrzzhyef.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gacxvcqoh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gssvhlkrb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gpelcntvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gybeycskn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmzbclohx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gpuvzyqze.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gicidntrc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gpxuxnjit.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gcrnbnald.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gnteitahf.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gxwaxjcoq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gwovjgfep.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gofyxjclp.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gwhyxdkfi.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/glyvchxci.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gyeaoeico.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/grjvptbin.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gepbadsfv.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gdshwlqeo.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gvovhmwil.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gqehrpabf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/guroijbsn.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gzmspgxbr.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/grtcimnlt.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gffhumekn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gdlcbtalu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gnwtogsua.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/ggmlmvhhn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gnvtfvgvt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gixjpuqun.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdivljehp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gfdpszasm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpadddfue.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gtdhtptpz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/giywkrmsq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gmhednayb.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gcluxryqy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gckeccpfi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/glgbnvnlf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gomlgbtam.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvqieagjb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqeeddcik.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gqnjfpmax.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gcbhcuoni.sHtML


<!-- 参考信息 -->