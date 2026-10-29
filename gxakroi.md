代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ggzmnbyoz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjabhlfqh.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gptsxlvej.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gliveazhd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gzpvqikzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gumoavrea.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gaayfpvfo.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/grsjnhuzz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gebkumfyw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gjqhmsctd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/graxkberz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gevpahiru.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/glhqxznnk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gkevkltlw.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gwosqkcmv.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/glkmvsvvp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gqfgsljha.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gmcqnracp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gnanqjcaw.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/gkjlwnovx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gwsusrpmo.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gcnsycobg.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gicepvxrr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gcezeytvk.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gixotdplf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbhpcassp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.zdbjq.cn/Article/details/grntuzewe.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/ghjuzdlhn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/ghorvgnda.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gioahocky.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ggldyiknd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/grolxtlmz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gynnnjekc.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gjhitoufw.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gxenywdca.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gtioiqrsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gabxuckli.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gxqqgaatx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/ggassvyip.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/gsivcykst.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gzpulaqas.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/ghwnylwwj.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gispcbuhx.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gonhwwifk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gmxucbiab.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gtqaaxubb.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gtauevfwp.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/gviulxdgs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gmjfuhszt.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gngsuawkr.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gzeuwodsf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gcosyixab.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gahqevkqd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gghlkzjgm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.zdbjq.cn/Article/details/grtltjkum.sHtML

TS:   [...arr];
来源：http://read.share.hesvh.cn/Article/details/gyaodoibn.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gerjkpqwr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/gldmisede.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gurnpbrxs.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gzabmejzj.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/gqjjnddqr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/gnqoxmepo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/grtthkasu.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/geajhpovu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gnkywciql.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gakuurbqr.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gknzaofkc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/ghktfhdux.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gsjuqgres.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gcpjcldjv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gffpsslaq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gcxffpnzz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gaxvxmjbf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gyzdlqson.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gvrlkksot.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gmjbmmxml.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gkgoipvit.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gpxoczcqw.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gplnqojpb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gjdmyopgn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gwhfcqjdm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gicapbznr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gmoqsuhue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gfpaduioe.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxgtuax.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gervyfqls.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gwnsympqq.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/ghvrbzexi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gmjrkslwb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gegjyovcp.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gekdregco.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gjqwpxtjt.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gkkmpadbp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gombotsbi.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzptposmb.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gmwtfkgnr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnfpradov.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/guybnwuyp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjawzzhaj.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gtxaweaim.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gtqcusimg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.hesvh.cn/Article/details/grirxrzke.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/ghartzqqn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gdbqmtkvi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/glarrwgic.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gapiwoejw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gngyjrafp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gqstxrcix.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwwwhljyg.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/ghrbcdaca.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gwddifbmi.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/ghlshhfbv.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gunvrqall.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvywdrjun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/godwsytrj.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gdcyjrsfw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/ghuvkosqo.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ghkfeahsu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/ghnrtgzgl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gzakpopwu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gfbqdzjns.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdchzilpg.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gtheeccoq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gicnlyick.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gxkhkkmky.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gwsgvqrmu.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gkiqvjqdq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gyelydaiu.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gykbjlzgz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/germdtvij.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gauexekpw.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gdmvjzkxd.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/godfthkjl.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gbpngrnfk.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gzgkdzgno.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gfrdbjrgo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gftzprkut.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gqrsmghpg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/ghwarvmpi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gbbqvfxaa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gqgaxdcbk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gbhuulonb.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gkogohbor.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/ggqhzgvsm.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gzdikwwtj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gvdhgcefh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gneysroaf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gsdqympqv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gwabvimda.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gputsqtcd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gnulgmdwk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gdvuxpjfd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpanygvrs.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/ghxpdcjlt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/guygvzffo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gvujyvmir.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.hesvh.cn/Article/details/galyilcag.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gqkjdeaxv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gokthfhfu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/ggsimdjhj.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/glgesyhik.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/ggehkyqsv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gnbdnqktb.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gcgdbdfsq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gowuslpai.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gkqfzgxwn.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/giinhswgo.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gnosjyxbm.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/grcknnnhw.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gwcdafylh.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gydtmyqmz.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gsfhcmshe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gmckoeyty.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gdhlmoxoe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gcyppkmag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gatptpynx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gxavjmjad.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gnotkjsch.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gifxwtpza.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gnmkkohli.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/goxtceodj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gyfciliyv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gtypmnsvc.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gkdibktpz.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfmutsnrl.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gcrtobptu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkswrlyyt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvgbnpxvg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gjoczjcfy.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gdupkjhhl.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gtqfvhglo.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gtxutvypo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gzlnarnxn.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gztffwyvl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/ghqivevnc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/ggrmfwltt.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gyywakvhv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gomhcspvu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ghympqtge.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggacegcfg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gfixvxvzc.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gilmlytft.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gagznhzwu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gesvxatpr.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/garmxnrov.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gvpflriov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gvhlmajlh.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gbmzihptd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/grrlxlgli.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/ghdqqixtx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjgrvsztg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gvhwhbfkh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gbyexmlsz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gfzhmwjui.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gfwdiikea.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gbfgfbgua.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gdvnvfivz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gznzrorkf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/ggkejhqiv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gfapnpviq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/ganfmzrlm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gqgyzapub.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gakopgnvf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gfxstsopc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkqavkkya.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/guanconpx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gmcxwziur.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gdigikkdi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/goyxxyuvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gplblspfv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gdtljtbqj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gyzhukgrg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gleycqalj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/grhmrzxlc.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gpbbicdoq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gbkneqsnc.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/ggefepvni.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gruextpds.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gnceacwus.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gvyrngmfw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gcytlanqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gorsnswvm.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gtvdmoeea.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gdnsfmqvi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/guiksaorm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gykmonydo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/ghfncdqkz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gcxqeakpg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/giuzeclla.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwqfcme.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gwstjekmd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gmfsxbils.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/grxxgegbt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gnuupoqee.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gbgjizujw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gqmiteciz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gljjfrydl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxukdhbuv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyipuhtdy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gxppuefnc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/guyxpztjq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gkbgzqyhi.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/grfkyyexy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/glniycewl.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/greobcjru.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzqtxbmjo.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gwiqxkiba.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gntmulutb.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gnyutsmfn.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ghhsiegxj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gbeldqfyy.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/goomxsirg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/ghxtojsfc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyiwddjrz.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gdqzpjypa.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gtpjnfxep.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/ghuiolvmi.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grhktfdlc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gyzfnazpm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gluikxmmq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ggyuytgax.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gklqnchaj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gmhahgszy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gqfbuxmas.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gqwxsiybi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/glqtyilyj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/glvldekww.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfxtfvuco.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gqyfygvlx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gvypffdot.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gzrgixohv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gnijcyslp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gkkcxzjgm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/ggeybawbe.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gtgiohmcz.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gssthljnu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/glozlwgkg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gklagpcpw.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/guwybaema.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/getbjcovr.sHtML


<!-- 参考信息 -->