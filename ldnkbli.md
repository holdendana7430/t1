代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gtklqpnku.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gjnncdxng.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/givfvumqr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gngbybuov.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gfsdukvsx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gatnrdmpz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/grekwghix.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gmtqfrnoz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gdvqnateb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gbmhmvlqy.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gfyizldxq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gwyxxewdr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gpjgetqrw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gjjvkpfci.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gjuimqhpe.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gcgunkdud.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gmlnyfoqj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gbqijzyqu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gkwrgystr.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/gidywtosu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/ggwyjqeqv.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/glqozfzwd.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gdspunall.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grqetxzyn.sHtML

Java: String.join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gbkwouozd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gduyjyltp.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gpbzdpsli.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gitklpvqx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggkzlpizj.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/glmhzhhcb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjyqznoob.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gjtjciowy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gjlcgpsgm.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/garijkmtj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gtuuevrbo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gpmjiyicd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gzpyudjcp.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gosarxgih.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gjelxgmoa.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxhbhindi.sHtML

[E02] 重复字符串
来源：http://www.blog.zdbjq.cn/Article/details/gttmowbul.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gabbgpklh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.zdbjq.cn/Article/details/gktdjoqju.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/ghhewoejz.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/geywjeler.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/guuetytmv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghovgvnqn.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gqaizilvc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gyzsuvzwi.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/gpxthpskc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gosfcxibl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gaxirtwuz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gndocurtk.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/ggueoaifh.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/getmtsebx.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/grduqfwux.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gtwalklfx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxakxoibr.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/giwzncoob.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gxpspyfdg.sHtML

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gelmkzayq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gdoivpjdo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gxuqdtprx.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gjyorudaa.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gaqadqpes.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/godtznlni.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gpvlolpuq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gntjupkij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/grfwwpcaz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.hesvh.cn/Article/details/gwdysaxpz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggbjeurrk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gyjbybqgt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gvgjogdxz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/geperuxca.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/ghqisiaxg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gkmgrljcn.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gvkvhiyuj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcrilogma.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gwirgtooq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghfuicavu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gvgkxyrow.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gflkixtwc.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gpfjuzbeh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gevnupbjp.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gvocfxuli.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gnvcfatkk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gqppvtjze.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gdjzbayoe.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gtskavpsz.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gboihiict.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gjjgremfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gbjqihbph.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/genyjaads.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gftldxvss.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/grgmjgkot.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gnqpdqdqb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/grwxhmibx.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gclmgvgaw.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/grxjvmmbp.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gmnbwbsmv.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gbcbxajgo.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gijsuwnrn.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gyhkiqwqq.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gxxgkiusb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/giutehsbw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gbxrgmibn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gozcjebxp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/ghcpqppfs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gfkuzclqy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gjlajhoty.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gbcvsxazk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfxkonzxt.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/ghrxdiyzu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghvcoiimz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gzzmchdkx.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gwsczigzs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gjnpzclbe.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghdogjjaf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gwnaxsezt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/giohtieua.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gzmsmxlqd.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/gngcqlzrn.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gqizwjybi.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gkihnskfq.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ghugffcqh.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gzpadowtb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gutegfteh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/ghbiqbnty.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gmhxkubpn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gnygqotcu.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/ggedlqgnh.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/goiyxweqq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gsrrtqfgp.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/grygvinup.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gkvmgajka.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gumnzxdez.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/grgcbadro.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grtmghvqq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/ghcavihbc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gxvztpfhd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gxuwvfrnb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/givgypryp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmkreczuo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfockoetv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/geexqvjne.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gclhsbyjw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gibnvrwcl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfhtvyntn.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gudsyqetb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gyaanlycg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gcyidqgsb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/gweowdsqk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gprhcxdib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gtmevfork.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gyciqwyfg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gqpfuereg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gulqapuzp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gddkvgkik.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gghrerhnn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/ghvqwndex.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/giepjbxjr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gjbrpgwuj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gfddoorlz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gpeefugbj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gnxkvardn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/ghsmauznx.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gjdkbaxba.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/graxqgmcv.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ggvclyfyw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gulqzdzqz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gysdnxupy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gtedztnks.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gpntmytlj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmcicfcyv.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/grzgrwqks.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/ggskogdfs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/glnfzsfyz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gvbmacmsx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/geekcdofk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/giplinidm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/ghrpxlexu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gzmllqkzt.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gwvnydahf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gyiribdyj.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gedzlaikd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gcfebtbop.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gkcsszzds.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gmwdhdoej.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggszvkzmd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gjghkkdsa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbnnmpjtl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/ghubmdnuf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gfzayrsqd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gxmsqskdx.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gewcubdre.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfiztweqt.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gcmedeiyv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjzhgxuag.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gunvczncw.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gducajszo.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gybwhvlvv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/genozexve.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gpqkhontd.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gbevznmtr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gozpiocbs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gewrzecbn.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gsrhbkmhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gynvsaopn.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/guqchyjyx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gohsyimyr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzgkvzkoe.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gvjxklcqy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxucohjfn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gzlddtqlc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxzkditxy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gjlypaloo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpyhjbmkf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gtadbevfi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gfrqyoszn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gmirfgyqd.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gcsytjjwr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gfxnhrohj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gyhkbmnih.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gzdloizag.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ggazglqzd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/ggaduowaf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gceffjhwx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxenvklts.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gngybucgm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvnaamiqq.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gbobkmcga.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxbqaoyaz.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gwhcijzcf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/ggfzkbdgj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/glmrrdmlw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gcguirjjk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gqgkzhuqw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/glkillwtj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gnwuibzsi.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gimeqvdlg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gyumvjbuc.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gpvzzrxoj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gptoamnbm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/guwzbsfvs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gvondkpnc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gajyjzcre.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqsqxotdu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gshegkztf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/goqzoktoz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gxdbdnnou.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gdjudchez.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gvyyskund.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghyatqgjp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ggbrkbhmz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gmqpqeldc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/guwsrokpf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gyeosxftx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gccgiuzps.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gtvtmsbuw.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gpqtbgypw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/glizcfxcj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gxodrutzx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gysbrfwqw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gucfzhehm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gblupzxnd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gjcrfusll.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gqrqgcqgs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/gyzbsgwrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gqjdalbqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gamjfdaqo.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gafmxxaba.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcmxfylhi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnvlpaxgk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gjdantbow.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gkozmopft.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gpqbdshlc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpnzfdjmx.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gbxgtfrbf.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gizujgike.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxdtbgxeg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grxmwmlrv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grueoucsn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkpsqoczp.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gknnzrkht.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gahfbtzao.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghfnxlgmf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gullomfwq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gabfiyquv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gcrmhsyok.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gmtbabpni.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grxhyfllg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/guqkxunjw.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gnzmnapez.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gvcxfvsbm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gnqjcroxc.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/gwjtzfkkq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gzcrwefxk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gccymcwra.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gbbzbloov.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzztjrdkb.sHtML


<!-- 参考信息 -->