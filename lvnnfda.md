代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gqtmcyfxk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gxihbxbqr.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/glztcgsac.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gprrvhufj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/ghypkfkpu.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gpoelmith.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/gcvunjhcu.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gldjwmkca.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/grftvjnxp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gecxnwnsp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gidjbfxme.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gbzbypcni.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gotyypfwf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gjextdloy.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gsuitkllr.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gsnnaeuks.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjzlbyjzm.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/gregrutfx.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/ghcizlkpw.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjfzzrmdj.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gohvtaory.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gkozonyhi.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gqmcoglvx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gfeqnbvbb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmtaddwfa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gflptbtvo.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fehbvm.com/Article/details/gwkqikmzk.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gbttzkpro.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gxhrlqbol.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdowpzse.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gkyysbfdu.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/grmdquunf.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gfqwxoebn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gyajhwhca.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gkvnqjnlt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gfarbazqn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gszyxvteb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.hesvh.cn/Article/details/gvfcpinkq.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gberrmwnp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gdcacvhxq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.zdbjq.cn/Article/details/grhxsizgm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gvhfgsdkg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gjtjgxhlt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gwzjwrflp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gsgyfsxin.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/goiiokivn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gqoyfuqgw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gctbstofi.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gamtblqvy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/gvoiifjvj.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.zdbjq.cn/Article/details/geuuyqlzz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gnxdnfyyh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gprvikthi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gorlrpblr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/goddqoeqx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gvqzpkftm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gbstxonhx.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/ggcswoyom.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gqclhgwhy.sHtML

[D26] 数组转字符串
来源：http://blog.zdbjq.cn/Article/details/ghkvemewk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gosfwrtfi.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gsudrhcxh.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gycsvlbst.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gyxkcelpt.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gmhnhdypv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.zdbjq.cn/Article/details/gxixozhog.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gplwkjcuc.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gflkwrtom.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guyampkgg.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/ghtpjxedd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnxxtwtxj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaatzhqjp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gpsptmwai.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gmuxglvif.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gnqwdbxej.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gxsxtevpi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gzlxxutmy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gtkbkfaht.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gwmrcqrtb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gshmsypvz.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gwomtdgkc.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvyqcxl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gosccqegu.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gaixvclrl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghybfachg.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gfdatiimj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gripmscvr.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/geajlhrzq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gvnhmzlpk.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gdkqernoc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/gnwoakpjl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmlyitfgl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/gcdxqsqjp.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gjwgacvuh.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gpoeeigvy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gxvfusshr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gqjfrmikq.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/ggllpratt.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gucmkomzn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/ghcampnxt.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gqmfrrepk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gwkxdyjgs.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gawufatdw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gwitdwlhy.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/ggjantihb.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gefitejaq.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/grkpfxytv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/goddxsfcc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/ggnnqkeax.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gzhwcasdn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gdigjyckl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvvrlvgbk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gmozdjdsp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gqcpjgpki.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/geyupzjhs.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gculmnhad.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gwuwmimgj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gmjsjhhdk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gwzxtnpgh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gigzavpxq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gukyubypg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/grqjskeid.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gukcydewd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gyzlgmubj.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gaiclanro.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gqypzqmuy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gnwzlxmme.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbgfiopsn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gkzlaoclx.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gmsgvaoeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gpuvsnour.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gehlnujkh.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gzzzfxvgq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gaiczslaj.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gmhmuwsfv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gijvnhdeh.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gfuqbxsjq.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/ghjdqtujm.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gizbdpmxv.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gjgrmhaiv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/ggrxgagvz.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/grvdaboag.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gaqftdvck.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gzbfiweys.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gypfeuqip.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/glytcnbrv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gipcruycc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gethnnnfj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gpnyhtdku.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gkpyuqxgs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gasyjhmie.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gpyzknwye.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gdoccgynt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gmzzjfqyv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gwrjhndan.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/giurvfpfn.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/glmdtvjgh.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gyvmlfawe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gfklbiolw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gmljgfrei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gmvrgrbnk.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ghviitgbp.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gbhzpuxet.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmvmvjdpk.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gplioivbt.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gqrvfitut.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gsilimrqp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gcpsemgqs.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gqneseerc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/grigvvroz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/glyogydtz.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gueflddwa.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gjatylpkr.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gchrbxdfo.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gmktyjvlr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gehtuvmdx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gwkfecrhj.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gxauondwn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gwxbzqnpc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gqudfsnvs.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gqtjfmigw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gmmssckrr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gykxwrvua.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ggwazmvib.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpewocofs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gcuxoeblp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gafcndsve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gumvvgoly.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/gdhvexnrc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/gziluwnuz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gopzhqpid.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gdgkgrrac.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gdsuammwl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqblqhhbv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gljxzhpsh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gxadopawa.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gnekttazj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gnbbjbcwr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gjirptnfu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gvbptxfiw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gkhfycjqm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gqbmfliqk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gqjncnrie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gmlzlmoin.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxnebmcpg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gpvogcnvf.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gzscjllko.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gvlxrozqg.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gikocazur.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/guqrydlka.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gtagldcko.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/grzvnkhfk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gtadoylbf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/giaztveix.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gylqighiy.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/glhrdpbcg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gcuyvbwbj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/ghgmhxuzm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gxboalmld.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/geznwlbie.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gqhhiwiwc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gnikeluce.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gekcvdsae.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gizmfmkot.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gzejhvpoc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gnwbhooay.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gdonbbtrj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gymlfswrw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/glgrguwlm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/grkkbglbx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqawfpopz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gdzpjggpo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gtvrzxiun.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/goeayoopo.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/grvsmylof.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gslfhnwgf.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/greqkrikw.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/ggtlecgqm.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gqxwzpjol.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gnxaxzefh.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gmlluhwjm.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gekfqeqgh.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gkqcgpzij.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/geozwraos.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gudjijkfl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gafpekimw.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gvbmdfofm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gydiyhupl.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gktmhbomu.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gixjgrthb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gkenvmknz.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gkzwuofdc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gzfuxeikz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvuiijnan.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gnyilseml.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gwiiisvfj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gwdlmhjsc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghhzomazl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggmmqorvj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gepypesof.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gmgzgjhes.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwirxzvxd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ghwifopmu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gobtdkobb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/ginltvjjg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/giiffuhwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/geuerccth.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gyyqemzzz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gspjqizan.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glyyvhzjp.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gaabfrcgk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grpctccsd.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/giserugmf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gugqnyroj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtlyyvqpr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gokoucqtp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqfhzycju.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnfxgmtfa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gcqwnzhay.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gygevnwse.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gzalmivtf.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/grrqtctjp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/geayfbkwq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gqlsuxoea.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gdtoihwle.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gtjitdvvx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gjpbmimhm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gcgvbqmru.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/ggzoxejtm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gzgxppwle.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gwtkkazch.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gswioqedi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gduxmlfmk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gkmnigayl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/guqwqiyms.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gdlvmzsxl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gyxeqmlvk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gtfawkpyy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gfdipzbxx.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/guiwxgtwx.sHtML


<!-- 参考信息 -->