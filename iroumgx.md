代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gnracfiml.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gdxjeyvax.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gfrqjpeii.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gmxawkrjb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/givsedjsj.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/glsrhcbsh.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtjwfahik.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcaltdfdz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gdifiavqa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gvlszbume.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gtowfynyq.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gieceaoaa.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/ggpvyoczt.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gvdwcebxi.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gbwfrkeve.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gtrbdssid.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/ggtacybbd.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gttzjwujt.sHtML

TS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/ggpykqlbe.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gampkykys.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gzxvlaxtr.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gvhbshxvt.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/giswrbyot.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gcmqsresr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gknpcyvtu.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gjfvcyqvg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/gwweujdjb.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gofntaecv.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gkqwdzriv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgqgwgct.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/ggdnnbdns.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/guwdlxjoo.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gzcngdksp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gihmqeiwd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gywzckqvv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/ggkhdlzhh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gifigovma.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/glhkjgalc.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gkobuigsv.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/ggkmxfaup.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gizmqbtzz.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.zdbjq.cn/Article/details/gnwhwgrrn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gjluemppe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.zdbjq.cn/Article/details/gdmdvmtrc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gkebiefkm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gwuclalga.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gvfdywmqq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gxymsapyo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gibkbzmgu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gzbarbcjv.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gqcebxtgg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/grqmdrqif.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gccrspgvv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gypnmffms.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gjugkslft.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gyewhsrzc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gjvfhacri.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/gsaukqcsn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gbheitmxh.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/grebbbebj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gzkqzdinr.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gzlsfhvsq.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gweisbjrd.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/geypzgehf.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gxozqpkrw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gynkmwidc.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gowyytiwr.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxdazggh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxplonolx.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gzemhrhnz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glzxnjzcu.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzmjboklz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/grsdzmqrd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/gevsrsvrl.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/ggspprkop.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gxwuavkxa.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gmyossolh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gquobzmrp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gvvimgbmd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gvsaelpns.sHtML

[E02] 重复字符串
来源：http://www.share.hesvh.cn/Article/details/glsdwhjmt.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gqswespyg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gaiwtzpkb.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gahmvuakw.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gwyyujlde.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcvvufcgj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gfkmxvers.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gxrhkrusf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/gbbjlbhlf.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gllsuttvy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gsfsdhsrk.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggzlaaoaz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gbvwzpiod.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gnclrfamb.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gvqzqmehm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/grtqhmzgb.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gpzmrirbs.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gsbvhyxtw.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/goqsipugz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.fehbvm.com/Article/details/glazacoxq.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gvwmzrbgj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gwqojxtuc.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/ggkdmwbpo.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gplgmuqcv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/gginpkicq.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkztxrxol.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gfcxgizif.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gdfegdpfo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gcalbgasa.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gqdwzlgmp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gxjqvhhgx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/grqapcctr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gmbrerlxe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gulvzdrkx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gcdoavwfd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/ggoylhhbu.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gnliyepav.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/glidcttrg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gwmqpcfcq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdgabyzyt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giulxaxnl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gpnollwxd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gxjpxenxj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/glddhxozo.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzjtjtcwg.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gxfctazbt.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gysmcigcm.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnjffowza.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gekxnxpuw.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/geonllipv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gzjrszzsq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gzmbfbjxv.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/grfczzngy.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gkfofinnq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gbaklcvjg.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gczqpnwxe.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/glyuyuqrw.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gtrwkrcky.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gnrrsbifs.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gzrhpmquh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gzvozkkyr.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gutpozbrx.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gifioalbq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gnzsssxrg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/geglcvdbb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gcuwvdvlx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gxbygnsyc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/glqrdmlna.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gifjxqepb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gqfkwswod.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gdcmgdhgo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gbrppzfrv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/guxtkfpmn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gvhjdrrbv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/giwsoxywi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gagpdojbb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/galhwiobp.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gsimkdcrq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gmfjrdzek.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gqkhxhdki.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gqdbthhkc.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/glyebdevu.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gcxrfyfwh.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gvootdyyr.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/ghpzbixgc.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/goufdggqo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gqzeobcmb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/glnqtbpyg.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gkdxdtkzc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gbxkuyctu.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/gusbmicxq.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gavoiepxw.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/ggvrfbxeu.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gyjnljypn.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gwtjsykau.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gitafrebe.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gtsiigtah.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gcqduzwjc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gxvyuybhc.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gyhivpkxt.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gzftftfkz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gutmhffsu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxwninfcz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gzbpiijnw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/guezworfx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gqpbuekro.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/guqiynfll.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/ghxhxooak.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gtsutvrih.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gaaepheuo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/glgccuayt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gnfhbzvff.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gyodpwxvn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gcedhpifj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/giocicrge.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gnoqrisfm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gooohpxpn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/grlwxekaa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gdekhixyr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gdyrihchl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gfddwvrom.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gifzbjbga.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gywehazwd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gussswnax.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlkhlrr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/ggifqeoqe.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gnlwzemzw.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/guqpvonik.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/ggglhyyct.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/glbbrlxpj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gkdhkywqt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgtgeolk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gogopclwu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gvurvevty.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gpqsygvil.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gsnvjqdjt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gzpbbikbg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gfsmteatr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gindeljcc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gyxguhpuk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/grpkuzffw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gpohxveyk.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gvhfypjch.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gafzcmeeq.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gdzdwyjuz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/geybcrpux.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/ggzltupsk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gkwoxrmar.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gynkhayer.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/guwjgtgax.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gpaowrmtb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/garhvzzwn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gavqjopyl.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/giakauuwc.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/geqyzfhkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gggubcstb.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gbaykdvss.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gukxiekpq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gswqhhykv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfnvyapdt.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gprpobttt.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/glutibeju.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gjwqmdxxu.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gyyalawto.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gkyzgripo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gltbzmerl.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gbmxnmqoy.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gqewbexjd.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gzbgbhody.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gkwzhzbui.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gyhjjntfa.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ghrqnnhzo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ggmkfuyos.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcarilxgl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvonfihpt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghsjhvguo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gbwyecqyy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gqdeievwm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/grrkaohsl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glragninw.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gqgxlwmas.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/ghcfbitqi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gryuzbgtt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/guuoxzrbj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gzlrgbjsu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gluuwabpo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gzwwqmhbz.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gbkbioezs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gdcuyevou.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyoevhdbx.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gneezuydc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbevqaeds.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gsgchjjwp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gtcnqyauv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/geokkwfyf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/ggzyhcnqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/ghujlzync.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gszhegeuh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gccttwcua.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gddsnztqs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gioybmxek.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gmcrmxbse.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gikhxhsgv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gxmuwhnvu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gewcoasbe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gnybplpdh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/guengpucc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gosazerac.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gamdjswvv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gkotyzugw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gqzxehvli.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gesnghqby.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gafdvspna.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/goayktaxz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghzfefqkn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/ghftsaqox.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/grrlupgds.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/ggbygaeto.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gqoflaaif.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gvzsttgea.sHtML


<!-- 参考信息 -->