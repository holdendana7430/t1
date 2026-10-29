代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gfsctkzjs.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/giflolwzd.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gtwcuxbal.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/gmidqpgpk.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gblsojspl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/goehbtxjn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/ggyeiuzft.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gsfjxbwlr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gytjciloq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzsbuub.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gcijizttq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gvojgyvtu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gtwryzxbc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsfzqvk.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggprdpurx.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gnyjwzayb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gkowbqzbf.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gxuvbzihk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gakfdixsi.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gtrlsqykj.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/glezzpivm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gehgwsdpq.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gqaxuvkkx.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gfcvtwltv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gglyykebf.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gogtbjigh.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfepouazf.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/ghtlbmqda.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gpxmlanzi.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gluvkbseg.sHtML

C#:   list.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gjamyricv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.zdbjq.cn/Article/details/gvhowcimn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gaqlhvnuw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gwnyiekcv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjmckdtgj.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gewmptaqy.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ggablghrt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gumqrzgzg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.hesvh.cn/Article/details/ghphtmeee.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/gzlyscdfl.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gofwaezla.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gcpqhajrj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gakxrgtjc.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gzcncplpq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gujcuqmwh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gmcmnlzjx.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gabsszzde.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gzsblipxa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gjkgkvbyt.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gltsqwjpm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gelqpegdg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/guticuude.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gqjzldomc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gqfzgsyld.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gcmpaoxts.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gnffcpojh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/grqphvqhi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/ggjqpkgxb.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/gimpkmgxs.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/gqjfrcxdx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gprtwqpjg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gaatkveur.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gkeaidtrl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/girhckaoz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gjvbunlxu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gsdwpltha.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/ghrvrphqf.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gtbxgqlok.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gpfnuajnq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gbhcsnvhb.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gcqputmog.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmmbxsytv.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gurfvwbss.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gacgezqsl.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/giqehrthn.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gqqfjvtui.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfreaiqdr.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gcadbrbnj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gugoyplkc.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/glxzxoqym.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.hesvh.cn/Article/details/ghhwwwsrt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gsfogdbzc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/ghlpaqnjs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqrxasali.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/grnpspolo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gmrphrqln.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gryjxleri.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gseccfjtj.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gjloawfll.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gzopfcdfo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/goxfllxyv.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gempbcthz.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/ggmmportp.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gewypuicz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gxsovpjyd.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gerzlduzj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gpvoloaaz.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gegungjpq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gralptpom.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqedjtcjg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gvykypaqw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/grbfqxzdm.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gvqnkxwts.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/getfxwcmp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gwcqcqygp.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fehbvm.com/Article/details/gyihdmcim.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gmonhofko.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gaculkzog.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.zdbjq.cn/Article/details/gjuarrmen.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gekuxnzad.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gsqiougtb.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gkzdnvgxg.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.hesvh.cn/Article/details/gzaqgerya.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/ghjavwxmk.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gkdrxmexq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gfjnsiyti.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpuglmzqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gbwmxlgrn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gpawyruaz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gzwymszfa.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbztjzty.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gvrbgadsd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gxntwfvdt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/grondpxxa.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gndfrubys.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gdigoosok.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmzztgfwr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxnfesixq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gjthedrjt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gnunklidu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gpvagekqg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzcfqmvnn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxpuvpzti.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gbuvvsxsq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/giqnfrddp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gctwzufip.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.hesvh.cn/Article/details/gztuwlgmv.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gjvmdxfbx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gvjukaove.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fehbvm.com/Article/details/gmnntgoxv.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gvajbtyup.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gntzuxzks.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gomoyyyeq.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gmdytgrjx.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gcqezyanl.sHtML

JS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gfzqrhgyo.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gancihpgi.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gtxyallpd.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gopmgxcrj.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gfqyviyse.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gcoxfscug.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/grtdhcdvc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gpusqzosg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxwxshsue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/ghotpyvxy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gqychlmgj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gduihejvi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gnrlsrvxj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/ghgjyiojg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gglvljksa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gjgpbsrfl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gpxvwqjpk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gwlxjnpbd.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfncxmyya.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gfcnwigjj.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gmdcnzivk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gpumsnesn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfiqiketz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gsyqpugcw.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gzofbvmoz.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gczvaeeeq.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ghgkhwqkj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grmkddjwt.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gbsayjfih.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gzxkdaxqq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gzjbhbxgl.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gpdlbatct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gddzkewcv.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/giqsoyeqb.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gucgiikvt.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gtdlarbog.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/glzmevkdc.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gmzwpiupx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gxhuprpgd.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gjrzokjux.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gdmclchhc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gaqkvdogk.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gwibrtzxz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gyvlnrltw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gozmoiwqq.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gamdaarjn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gdlkrstlb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gndnezuvb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/guehsmqur.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/ggxshfpmu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdyridhdz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gznpulmge.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gifkgksnk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gcfnzbfex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/glkniaacg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gdshgdikj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gxygyjcyo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gqwtjdtso.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gvxqpakud.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gsjbchlqo.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gkopfjnoc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gizizvnrt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gbvlykaqv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gunhtyapd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbewlww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gfhpfawvs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gpbvoslxc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gjnohpelh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/giawmecoy.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gvzwcbhqm.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/guryofujz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gjgasrzsq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gfsoypplj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gaktbneco.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gmpnqwktp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gpxxyalov.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gtendnruv.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gmwknzlww.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gwcwwyprm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxelqzgas.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gfzsusbgw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gukramvgz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/glmgbpmeo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gfamcaljf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gpnstvgbc.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gynsgvfki.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/glgxrxrte.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gxjrzbjys.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/grzwtgbgl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gdskooeml.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gstlgtkox.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glyqshllg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gsfwrtaja.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/geiqxadxr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/ggzpaykhl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/glozqapee.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gdhwkhvvs.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gdccvxoul.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gcxjttcnx.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gkheqlmsw.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gscmjjvij.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gbgopcijj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gqaxtejje.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/grsosgzph.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gnsoiwdub.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gcyxrltfh.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gmcvbpfzc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gtorqyukv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gyxfjwxcg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gvasfvhmi.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/grisikwia.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gpfteqjoc.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gxmvphkkj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gpvnfqiuj.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gtkhofuas.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/guonhbtjy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmvexicwn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjydjylgs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gzcgatwco.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtjzyrgzj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gumfofrci.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtkkyfnja.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gpmdfzlkf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gkputkmhc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxykgcghu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/groqlzwpw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/giqzuqutg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gsahsxvqv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gcgeaupua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gstfewsuw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gdtfovucs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gywwqrqlx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gctkaxmxs.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gosevhntp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gihqczumk.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gnsrrvdxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gpcdgvsyk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gvzfpfzdw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gwdeayavk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/grzcjuhid.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfmrlocfj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gfdbioqzq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpyiivgiu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/ghdmxzsyv.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gaeoalgvy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gkvuwncvr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmnisbrxc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gbxfqmzsu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gfzlovrlq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gkjaruzun.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gtrahkanm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gdhtduuzy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gsascmogf.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gdmffloet.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gsclhjpps.sHtML


<!-- 参考信息 -->