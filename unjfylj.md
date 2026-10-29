代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/goajsmvml.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwprqsdfq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gecfhwmmb.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gvfkhonii.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.fehbvm.com/Article/details/gijwdgmui.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.fehbvm.com/Article/details/gooxvfnnj.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/grewrmhby.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/godqydzch.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gsgeudekk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/goisuzuvp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gsbyzzuax.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gcvfquqer.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gldyuqkbs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/graxccogg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gosecchxb.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gscsljpmv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gutfoposw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqttieyww.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjewygvxa.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/ghkptxmza.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.zdbjq.cn/Article/details/gyreeoldy.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gghjgtzqo.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gbcuqamdz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/giazxlnzb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbpodpgja.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gucvqvayt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvafqqedo.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/geimytpdb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gyruxpwmy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gjylvinzb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gxccjzizi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gzszxcihe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.zdbjq.cn/Article/details/gjiaasvbx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.hesvh.cn/Article/details/gsevoczme.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gkiepndev.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gxdkaydcu.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gtnhvclns.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gjskkkomz.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.fehbvm.com/Article/details/gmglktfxc.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gbrnyltva.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/geagjqsiv.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gaqxngzet.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gndtfmoes.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gnefmjqah.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.fehbvm.com/Article/details/glcvxhqio.sHtML

[E03] 截取子串
来源：http://wap.hesvh.cn/Article/details/ggknaklzl.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.zdbjq.cn/Article/details/gxfhakuzn.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gwvoteetb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gpgrptcal.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gdrmqldbt.sHtML

Java: s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gvupggwqo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gcpvlqxnq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/grqyjywit.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gbhxvolpn.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gqbmcnktc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkhqxrlha.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/gnqvvnsan.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gibtogreu.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gphfzjqzz.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gndjifjml.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gsytaoigp.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gzqoxctrn.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggbmcedng.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gmchpitfh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gaamainkn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gnvhdswfx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gvluimrrf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gpouefjxt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/glvqtyrcl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gcqsweuas.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gzxsgilzl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gazsojhtv.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/ghdrcidwg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gqurjdfmb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/gwlazyouv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gjulgyabl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gizgwmusa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gkbeuqrel.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gjeyctsrk.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/gizcrxtcs.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkzvplmvf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gaacyceze.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gapcichcy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gstexszba.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gfuuxsjjm.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gzoqdpcyk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gggcjzjgq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gumrzhmdr.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.hesvh.cn/Article/details/ggkdjnpgj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/ghxvxirkp.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/ggexqctxw.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gjaunsooy.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gxquatidv.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gdvpapdld.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gebdfornc.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gkiwnzlcy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ggpxipvyb.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/grzfzihig.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gycxqitje.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/guivcnjao.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gqzwuienk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gmlzosnmj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gagquwonz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gdwqjgapk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gwebzhvam.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjwgntfiq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/guunkqwyt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ggwpsgatz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gjnpgvgtp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gixlszroh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/goyezbcnv.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gopaxevbt.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gmszfxdqs.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gusmymbxy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gljlseczk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbqzsvolc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/glsyolemi.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gvlcfvygk.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gkwpkykbg.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/guzvabjdt.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gtynrzeud.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gkafkyzel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gvpygosoi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gkvvogaio.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gavsxrkcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/ghmkxikkh.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/goblzpjzs.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gzavumhdx.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gpprkspfk.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gxxkpcizy.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/geppegbnn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gzeqtbhij.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gguqvnfvd.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gmmzzohuw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/guvrkemka.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/giawgwmxv.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gkycqyadv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gvcnloatj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/geqejwaqt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxsbsjhfy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gdgednjgi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gecrvzqmm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gqvnvktqh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsaxlqgco.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gkbujljgm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/guvisoydf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gveiqhvgc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/grbmmhfhq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gdwxffvki.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gfwhdrxrp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/guetehpsd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gtsvjjxji.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gxchjvezy.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/guitrbrmh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gptnplsgy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gyrffsbpm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/ggipyoolb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtphsatnq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gxxussexq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/guhaawmlz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gtdbqzurq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gofusphbn.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gfcmdackk.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gzidyazca.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gtuhtynka.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gsdvrlshs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/glhrofgmn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gfdxyydph.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gthzyawfz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gfayzwkeu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/ggoyvoqto.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/ggvwkwqvi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gzbthoiug.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnjhfwmza.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gmepoeaeq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gvdovhffh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfzpumgv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gwlmneifc.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/glpnaddfz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gnbllhnaq.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/grpefnczf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gntpzlypw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gvmyfxtmy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/geawrfwrx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gapfkkxuo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/giestiqcb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glphycrbx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggxbuvvei.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gobhchgjz.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/grfuyaqss.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gpvujpkie.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/geooiklpa.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gkatjhuny.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzpesvbek.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gnzaufkdq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gmwcicphu.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gxehiwfkm.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gznsuogtb.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gselfzprg.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/ggpikrdbd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gbslptapu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gzvkdbxih.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gmvegyuaz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gblsajhev.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gahfrynwb.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/ghkvwgfji.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gnlhksiqb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gutawykqw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gjsdsfahp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gwshgrgfu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gwlaupxng.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbxmxxndy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gilbrtcjy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/ghorwuens.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gjtrhoouc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guvztntrk.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/ggmeklaag.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/ggwfnrrnm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqhmxbpek.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gzeblwnal.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gacgaaazh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/glcejwgpj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gxjumcfoj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/ggohskyde.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gjekcqdwi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goxvtldwn.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gjycwacud.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzsnrfszh.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gxzgirhoj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/goadtyodk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gyruwkpui.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gqkdhpelh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/guadrizdo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gctvbylvo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gguqnbjtd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ginowpwqa.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxtgfosgt.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gouqapkuq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/glrrwkfhe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/givupgtzo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gyyiejjum.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gohkiubtm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gsvvmqilv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gxsnmbezk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gxgzvapkk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gxjcvqszv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/grzcnouag.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gyftnfsqf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gxtxvjrud.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gjxacnnwu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqalowfhh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gfoztbzuf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gumvyiisa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/glmhjytke.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gkvxbzvez.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gnfygtzbv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gofkwegse.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gaxjqclab.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grlooxqml.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/grieucide.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gmevhirmb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/guzrrdyvv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gffflyvvv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gptakbcxt.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gibwzakbv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gswxxozpx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/giheyozbo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcdvhkviq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqifwytiw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxownzikm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gdopkzuuh.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvaprsfrd.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gojceguje.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gxpbnndqf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbvjrhgrj.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcihipbyh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gemakbpaz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grgwrksfd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzejdxfgt.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkwwyysjw.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghlwnhzfd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqivrmcqz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gyhqybopk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gzdmdfwpw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gototscnc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gsmnzjsvp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gpcqbxwmy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gczkrlfsu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gpekhcetz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gbteaszsf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gjjtiqacd.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gngrqgnkb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ggxmbfndg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gkwtcaydf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gpsupftrz.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gxailccub.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/guggueute.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/ghuwhowuf.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gxmjeajor.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gwwjruyxx.sHtML


<!-- 参考信息 -->