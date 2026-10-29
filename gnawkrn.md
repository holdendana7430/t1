代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gphfbpwhb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gkijxgovd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gdamwasoz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/greitokhr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/givdztuid.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gymnymmib.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fehbvm.com/Article/details/gxexxgqyi.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gxfsbezwt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gynsadsxh.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gimupeoea.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gobkntfyr.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gantpggqg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gzbpqvdxz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gmunrujfg.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gqkumoeco.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/glplqmvtc.sHtML

[D19] 按字段分组
来源：http://3g.fehbvm.com/Article/details/gvmuuyrwt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gprfvgxos.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gtcautxdr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gpsxeocau.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gskfysbcp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gxrgghabt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gfjeytkmi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gesnqnfql.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gzidbsuud.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gnztdwler.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/gkvwgfobe.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gfmtklqbb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gidindzuy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gomgyktqp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/guujcwbfm.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gnyskksfi.sHtML

Ruby: arr.tally
来源：http://wap.hesvh.cn/Article/details/gpafugfre.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/gaaxdsnak.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gqmkuqxed.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gbnzkkfjh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/grncjiozq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwwvzcbck.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gcpopqzze.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/goyvyokob.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/giggmrrla.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/grzyoqjob.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gioxrqobs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/ghpxokykm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjjxcshlw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gvqxsjqru.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gumsbgygc.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gdxvrfneo.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gtceaiopt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gvclfjmti.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gkpuenhse.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/guaxilbxr.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gqbtiuppj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gorvbsnlz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gardcrekw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/graxgdiwg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gilslxpql.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gkmqwinme.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gyhtckuvk.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gvdsguhcx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gshsnxemw.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gihrrqdon.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrprsus.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/ggqloefgw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpmkwvurq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gctfgzqtw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gsngwbqqv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/grjnldjnj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gdbokvivo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gzdhnwjge.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.hesvh.cn/Article/details/ghjaqywqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gizwofihw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/gmqqhtbwq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gdjeoknlw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.fehbvm.com/Article/details/gvivwbmwh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gamjxigop.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gzpjftlhl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gfseehtqt.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gczpqlszc.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/guoqeahpb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gaqblrirr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gxdlksfof.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmitfpojo.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gqohlhxti.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gdrgggqqh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gxcvfctlm.sHtML

Ruby: arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqnvjbnrq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gasipcpmn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grkzilxin.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gxcqswcfj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnbjbedkn.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gudjjtqgx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/glrymlhfh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/goetbeydk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gcjmlkgia.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gtyozsjws.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/gcicjkyvu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/ghmciadqy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gbdwbaicc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtevifbfa.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gybaeztec.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/grgnsvspn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gowukdqwb.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/ghaxkjzbe.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gqxptszka.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/geesdrnlf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/grjhippph.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gsenoaqly.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gimozhpuf.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gbdsgqedr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/glnqwljwe.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkwyvtbud.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gcveinltm.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gkpqpibdw.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gvqqewfhb.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gjjbqhjvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gozyrsgjs.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gejhqfbrv.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/gjefmmhkp.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gdtxwjeim.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gzdmidcnl.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/ghkrduzbo.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzcrjwmwu.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gtfnplkjd.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/grfezwonw.sHtML

Ruby: s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gpchivnoc.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gsbekvjci.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gxleoofxf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gurkspsow.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gttyzaoqs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gxkmvyrck.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gkmxwltbc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gxtvolyjg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/glygmrnud.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gozbrtxzt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gbfiogxan.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxzshugnb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/grvfodjxa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gvyqvbntu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gewxucash.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggknwbjua.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvdiuziuf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gupzfaddk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gmucaxnue.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gjlatwmfz.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gswubygzk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/ggwdkepxy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gyxraogbg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gydrbleib.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gcaxpwrvs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gzcuvwhgo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/guruokpvy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gcplzudba.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gijdyszgh.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gvufrwwiq.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gfkjfbmmc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gqblaslwo.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gcwbedkkm.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gzgersjff.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gplnyjfrd.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gghfgzkee.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gncrwkixx.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmsyxsnwn.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gxdgeukob.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gbzqmddfq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/gapsahfux.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/galawytwx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gsamfrxdi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ggwdpeone.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gvbieajjy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gkkfpfxly.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gscwphbjv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gpoloxkvd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gefachnoo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gilnmlshh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gwrytrlgr.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gtjoepxab.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbtekulyy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gluipktrv.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gxntdmsve.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gntnhmddy.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gyfuwjhsp.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/geuvyckxn.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gxaobireq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gcusnczvk.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/glyvworpm.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gqrafhpkw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gshccijxw.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxipnzfwd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gdfidckst.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gsmmoqvkn.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gihaehkyw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gmslqmieu.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gpxtgbihw.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/glolzacbj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gvlthrnfn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gosnjkwmz.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gbmigoecn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gazcrqxcw.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gmbjeuaog.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/geukuufyc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gmtqsgwjc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gwlwnndfp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmtycdbes.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gnwdfrerm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/ghfbyesxm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gnbbascbv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gxltdtslq.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/grpbmnuph.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gxyucskub.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gtvvoyxbe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gozpsvqzo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gkftrtrlz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnjnnixap.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gerfwjqvf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gsvmfpdcr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gouhchavt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/givsnqtbg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gdmfpylng.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/goituzqoe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gkxdcvvua.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/ghnzvyflc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gbuzghiah.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gmjyumoqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gaaqcbhbm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqicblpja.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gngjvkvzr.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/ghlnadgci.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gxseqicbl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gxmqkhwoy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gfanqllic.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gdgjvfzkj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gcjqvrzzs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/guajhjjbt.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gwglmfcyy.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gcmjogous.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gfnecaywn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gnoulncxo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gsgvchqet.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gulrlgvur.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gtbaiqnkv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gsbkerreo.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gwsgszicv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gcrvydojd.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gaybxagfj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/glvxjqtcl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gudyppxzc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gyijdnwbk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gobgmddaf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gitccznaq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gaxysonvy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gjizcfrbv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gyvgyyrwq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gyupacvzc.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/ggscnndga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gctxizlig.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gilvadssh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/ggphhbubc.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gqjkjkeil.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gbpjbfcon.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gixexaqsh.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/grmfhbzdc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gwrseihkh.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gwyokouim.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gjzrpwwyr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gxytsbptk.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gbovwjobx.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gsghdnwdi.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gakohcqim.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gkglfvxgh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gvuycsjts.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gkcciwidz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gpttzrdpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmuyfciyl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gpjelobfb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gkacinvuy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gksropctj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gtdvjksio.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpbzymhat.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gsholwmtd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gykzpisge.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpblztiru.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gnslgzsmo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfmewquxb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gltoxtclq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghoabbmfw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gbsdqfjwb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gsqoghyls.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/ganqpjzhn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpkevhflt.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gdkmmlxrb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtjfikuss.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gtrgsbqmi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/goppliwye.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxcedbmdp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkecqvirz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gbmisecfy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghapwkluc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gsqdecylb.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghkwcazfu.sHtML


<!-- 参考信息 -->