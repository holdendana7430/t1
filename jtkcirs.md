代发 wailian999

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gqlhpomyz.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gvyaibadi.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gkpzuzfzm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gyqpcdfms.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/glvenlcme.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gecitwxzi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.fehbvm.com/Article/details/gosdozafz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/gjjevuspt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyswisssn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gpzpzjxjx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gguoinour.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fehbvm.com/Article/details/gatnyuywm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gdftzfvlu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/ggrbjugks.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/ggrgcdpyc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gbbeaqepw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gtcmkhkcj.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gvhajdhwa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gspkuqyju.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gepooidld.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gwqtlnthw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gttonqedo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfvkumblv.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/gwjtsojec.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/govppyvgc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gwipecyue.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grvyygxob.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gmjkrhpnt.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gqyesuouk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/gmubjplqz.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gfcedzwhq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gyubkmntj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfdtjcmyb.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gxpqxxrsn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grwybhrbv.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/ggqshavto.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gqcorxncy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gsebuplvn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjtdsfnha.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvphhxwus.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gqvnjwhau.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gbwqgayuf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gnvfoqylr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzsdtsm.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gkpyteunk.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/grjbkyqfq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjsvgajhz.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvlymthng.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/giegndvpx.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/geqozlvhi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/glluoccee.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gsjtfkkyz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/grpcmndvg.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gcuepkqso.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gbjarddzq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gmzeqzmri.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/ghevlxaws.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gemiymerj.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gystasmde.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gvrjpvjxy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/ggcdsvsdm.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/gfeffucvq.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gmskdpjaz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gwgdousbw.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gdzmamxwz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/goaympmxs.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gqurdabgv.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gexqdrgzm.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gkhoncier.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwpjeenat.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gbyexodcu.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.zdbjq.cn/Article/details/gnqxgewus.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gqjdeeprg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/guxfmcsan.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gyepcspgd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gapzqtnct.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmpsvcwmy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/ghiknbibk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/ggspbtxba.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gfmkzjqpa.sHtML

[E06] 替换子串
来源：http://blog.zdbjq.cn/Article/details/gkzkpjvyj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gvhiflvnn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gwmfnrlde.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjodixxry.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gycbevpud.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grngkbqey.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/glwsaznpa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gafkabcph.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gclcilodi.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/ggvubpalq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/grhysoaah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gqtuktpqt.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gzsqgiigo.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbbjmajny.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gsotofatb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/ghrdodrgj.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gntzljwwk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gboctqrbo.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gnjeclvoe.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gpjnmlmlk.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gltdbpagv.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gxlaexxtd.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gpfmkbsds.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gmjtcnngv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gogjgvzfo.sHtML

Ruby: items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gyiwrbkax.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/ghqjgauwq.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gqzoxfyxi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gdvynkrnq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gxvbvuvue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gpupqrwnz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gbkowfyvw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gvbsotydi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/gbhaxrpfe.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/getadnbkb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gecpsfbws.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gienjfqqo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gaavemkvf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghhwwpeau.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gzkjxblce.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/glslvvisu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/guqsqjubj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbnvyumfp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxlebwxei.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gnfagzwkm.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gyquwbmxd.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gyowbcexf.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gawedcjsn.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gaderdiik.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnzcdadgg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gpqadhtsg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhcdkvs.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gfvswdlyi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gzrramjls.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/ggfpierlb.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gawwavqck.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/ginexkarx.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gadwezmbx.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gfnemfwxa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gfvuvrimq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gqjpbqmdd.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghzpsesvs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gucyjizni.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gzfhivfpl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gfstxcdhb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/gkvixesgr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gfqewfxpn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gapsmygab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqfhurb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gfckbeefh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gplnxdppq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/ginybrlkv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gphxmlvlh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gboghdcvq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/glflvmknq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gydiqkzks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxeykbl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/ggxerqsiu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gxwaamsmu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gngnyzyzu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghmjslwmh.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gfauuvuxe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gtnriabbx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gbtbfrhix.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gvghtyxxa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gabpskqqj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gompiubwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gneczzldj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gkmkgsmts.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gaehvriyp.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gflbpcshd.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gfvgxpxia.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gzwcibgki.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gxyusndpz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gcqftteze.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ggqehesyf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/guocdvfbi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/grpwvdexh.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gncfavtvo.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gxsgayocg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/ghogsngpp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gmxzcfcdv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/ghfgqirdx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghcipzgho.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gtrhxrtbe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gogdfijis.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gtxdntnub.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gamikanid.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/ggsvhftkm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gzfirainc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gcnrcllgw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ghqodtzcr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gafznegtf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gfafxvkxe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtxiznsnz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjyfeodnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gbaanlvhs.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gqurikhbp.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gcbjnehrt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/guobreuxz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/giushehen.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gbewecunt.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gejaxxlhb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gcjierrsy.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/grtzvczqs.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gpgveidns.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gbistokrg.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gjtxabsoq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gofnevhxd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gqrbmenhb.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gvbiyuyyv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/galohxhuw.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gijmmqtzb.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmfdkjdsi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gvsevsgro.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/glgwtrmha.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gbqdgyykc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gymdpzpdt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gahxdvnho.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gyiubevra.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqtpluluj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gkxdqgptc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwdvlzypu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfnvfzzzd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gkqqxlhmd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gibiydvmq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkmvwotwr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gsutppslb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpjewcxmq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gcpujkiqk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gmgsnejeb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gafqrfqkq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gwlqmopgn.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpffbzujv.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gkddwdcli.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggyztzjgt.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/grdcdspji.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/ggtvtryoy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnvmkqrfs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gbxciuefe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gtgxdjcrm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/glkujvnie.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gvtuwhgbp.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfbaahysc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gajwfzaiu.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gktwisoym.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glnsqtwvt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/grdjiqoxv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gdrtcyqex.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gsftdthzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/givtyowyb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gfsvozhbu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gyzetucwi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gwmmjhtun.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/grujdyzyz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/ggzyavvik.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gwoumtifx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdnujyn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/goksshoqe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/geohmdksl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gcxlzwcsi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/gpgqxrafw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/giowczdmo.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gfrytkiuf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/guehzzyxq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/giqfobtpw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gphiqihdr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gpalixuet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gmxyonmnk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjywskaff.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gnmxqphyo.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/glikhatnx.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/ggwfvzmfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gewjoyfxt.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/grrbwvbzb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcezkzydy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtcinydix.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gnghjdbqg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gmymlcfvr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geaoksgzg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpsqajkhm.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gowzdqvnv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqlyyczah.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/galfcvfaf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/guhqdpkzl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gljdopeor.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gizsebyjs.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfhbtfrtk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcuhlwark.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gtevmohtx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gaeyejszz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gacjhrfmh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/geddcoddd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ghplpyozz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gotzsyogt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gyemauiug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gsigmfxzz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gzjkofcls.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gslhaivnv.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gidxprxah.sHtML


<!-- 参考信息 -->