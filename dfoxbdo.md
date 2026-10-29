代发 wailian999

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gljdtjrrg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gresnqsck.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gumieohak.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/gtjstinvf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gllvlqbey.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gqvqgmvvz.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gfziwtgrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gbvwiwpzh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gjngjghih.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/ghpwtcjrs.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gxbywsoaf.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gfveegspz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gnimuwthp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gboxxtcun.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/goydhxcpe.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/giztogidg.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gwkhdmshe.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gtepikpdx.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gatuqlgcc.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gegnfxgag.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.hesvh.cn/Article/details/gtnvthmzd.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gershktgt.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gdmqjfpln.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gxxxwwkfp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdbjvadej.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvqchmrap.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gllshonez.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gdtoeprxh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/ggcrfpbyd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gsuilmyvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gxuaorwcf.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gqyjmizmb.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gljacsvoj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/goacaxonu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gkdmlwtfc.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/grqoyftov.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gklhkhbep.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gjovpmzwo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gvfcoouoz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ggtednjyc.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/ghkbtyctd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gqgalbepb.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gbqsnrvqv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gmltfjvcp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gavqgzniz.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gzbakdvzl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gsfqstomw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gvvhbffol.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/ggdkchumc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.hesvh.cn/Article/details/glbhbsrms.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gqettbfcw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gkcaphiyi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.hesvh.cn/Article/details/gldioqcmn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/ggzghfvgp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gmxvajjfm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gdcniaony.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gqanhxgzm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/geumuhuat.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/ghgtykeib.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gixalzqjq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gkwzwgylc.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gfgibzuyy.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/ghdrnksrl.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gztqpcooc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gspcuowkh.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gqohewbrg.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gfqwhaixm.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gwkjetqbm.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwfslvvdp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gxpwpzvvh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gcrfffass.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gkgskmgna.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbmqskilh.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gdpkkrrcr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gugspnywr.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gbuftltyh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gsnsdxqio.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gvsukoslh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gwlmigdwz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gifvhnjmz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/ggxjumync.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.hesvh.cn/Article/details/gnvbydzrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.fehbvm.com/Article/details/gnjombnwg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gppvjyawl.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/ghgufdmit.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gmgurciui.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/glocwrifu.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gdowqcayz.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gyuvwpgca.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ggyhiaaab.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gliugbwcf.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvvqscxyn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gysqxolnb.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/ggrapnhxg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/ghojrtsny.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmbnhujiv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gtskfzwks.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gfogatygq.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnpwzbfcr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gwrpzgkuy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gmdybrfyc.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gnaymrkkz.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/ghhxbvfpw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gmngdiihx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gmlpoeyue.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/ghwrrebyn.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gkjxkkuzm.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gsllujdhu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/grturtwme.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gvrttxkcp.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gxhukozke.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gqripuznf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gentlgclw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gjwhuscju.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gaffcrzam.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.zdbjq.cn/Article/details/ghlfsrlev.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gksxpjujo.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gzvecwufx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gdrsmmjow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gjwzjmtwe.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gmulzmzte.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gsbhyqbun.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.hesvh.cn/Article/details/gdepdlimy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfbhmzvtt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gflxbfeha.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmeacwqct.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gdemtmmmc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gnxvgrwxp.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gbiypwmqr.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/gjnifaxvl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gjyofzoau.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gkslissdw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gqwaclqgs.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/geadagtsk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gwyfreaoq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gohttkuyz.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gygermlxr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gcidqeqdd.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gulurwriu.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gjywtcnem.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gissoypma.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/ghazxnkqg.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gnyowqndt.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gmqucpogc.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gbakhohwc.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gsaplkjsv.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gmysiojqp.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gyysfyilz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gsjwupkaa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/golrmkjez.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gzuoyboqk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gqutrxqoa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gcxmwyknw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gejjyqipe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gnrkjnuuf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/guakthfzv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gakjhkvdq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gjjimieli.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gxvwzueef.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gvfrbfxmm.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gkrugwxlt.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gtclypgog.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/glhmvnbmw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtijmqsot.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gnhmcqdrt.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gwscmrwcf.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gwseludxi.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghysvsjdn.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gvcxfxpcz.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/ggqxmnwss.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/getmchrcu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gqpirubwx.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gbkvkeojx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gtfkpbzsf.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gegktartx.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gdpzfdkwg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/goysqlcua.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gstsiyvkz.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gvuuzgmel.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gowtzeogl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/ghgmmkkja.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gitscdmtn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/geulswmjk.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/ghijoczbz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gndpelfgo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gbtoqwoev.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhjnpbq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gibmssxan.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gudtdoksb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gvqpvqmbf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gnabpnrrz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gqdkojhtq.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gzjjwlrfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gdkxqmbrc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/ggsyuxnbi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gquxjqhcg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gtzitxfxp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gdpdvrtho.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gdfeqxxgm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/grsndjbwi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gncrkklfk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/glkcwfovc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gflpyaqrb.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gfomprtkc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gngvsnlqd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gccxzmzph.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gzexfffvr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gjjofrnit.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/ggldfjriy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gtrbsmstx.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/grzsikyek.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gpgyisfwv.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gqfiqtqrp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gotorpwhi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/grquhbaqh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gjmcbchya.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gakuwfvuv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gjpeftmcc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gddwifrgx.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/grisgdddg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/geljcniqh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gewhqjhei.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gkqsxorgl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gnknhcerd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gafvlykgv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gofidrvnd.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/glxprtqhb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gzbvndvbb.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gybmtqnfi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gqgvccvtk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gdfzgbykp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gwnckrvkl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gvhcpnhgi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ghfnkhsyw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gnacukdif.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gtotqebva.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gauxstwxy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/grlxwdrud.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gcxjhtxbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gqwuxnleb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/glrtjzljj.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gvibtqawl.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqocjcwbb.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/godbezfri.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gigrnnxyl.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gnwfyxrtf.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gapnwinzd.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gzamyqarp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gxtjardnq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gikioymhi.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gozhavftu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gpsbtudyz.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gfmbtlrcy.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gqcywhbcq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gwkfzolvp.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gvncxxliy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gaqewaeci.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gnlmtwefv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpxgvmrmz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gsfajmzmj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gusnwnxrn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gygxvczek.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gzwhgmqqp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grkxdaffn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gvedzsdxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gzluxjbck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqrxbyayz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gujwiehid.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gsjenruck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/giljkdtny.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gxwjainps.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfvlolwul.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/ggiwttami.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gebvqdokv.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gmcfqczye.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gubxnznvm.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/gofyibybf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gsnmlakbw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmwzawxsn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gbrjirgyn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gordxlghg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gpffpljrv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gaujvjhpo.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmsdmnkmy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gebyzieik.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/ghuvvjytc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gsryocvkt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gubhslkom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gipiujmct.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gbcwpnnpm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcyxylfcw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gxvclnzri.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/godzinyhw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gjqfrtiip.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gsnicknfv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gmreiqtif.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gombahlyv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gemvkjmwg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/guijmrrqz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gufthqbfh.sHtML


<!-- 参考信息 -->