代发 wailian999

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gkoioivdm.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/gkrztgrwn.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/glboefona.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gtdmhaonc.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/ggfzaphqh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gwwlkyrsc.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/goenzkygz.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gpmnmpsxq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvfopziqo.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/gwlsxwwwz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/grhdalkrn.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gnfebtgno.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/grghpnlbw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gtiamgdju.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/gcytmbxfm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gjstyxhyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gpuqovdtu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gvjcqnvau.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/ghbevwwvb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.fehbvm.com/Article/details/gdnqtchsv.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gzcdounde.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gsyodbwvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gvajjpnwx.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gukjjwgiv.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/grqeymmyw.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbjlrycwz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gbjlbncfc.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gogowafvo.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gnidmvwzy.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gkiaulqmr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/geuvsrjxx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdddggnfj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gfrngffyz.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gfrwlzjnj.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gjuydpxlv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fehbvm.com/Article/details/grfsbrpsc.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/guclevxmf.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/grqkcxqsv.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/grrmvsmng.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gugdnsvtk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gxvnndfux.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.hesvh.cn/Article/details/gaqwnavqc.sHtML

TS:   s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gwmptmkze.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gjfdhqhvu.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gbcyertpc.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gosxwtchb.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gnrghyutl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gzsmfxvpj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.zdbjq.cn/Article/details/gmcyswteq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gjgpgmvrr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gejrnaaxj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gimrpxyfe.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/glimvvama.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gadlooimy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gzksntiks.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gunhmvftg.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gfdddurjf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ghsevwyim.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/guklqumxy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gxrmsxuah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gukorxmua.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gffwqymmk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gmqbccfsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/goualfzyu.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvrhyazii.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gnboobmwa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gwozmhodo.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gtbugnqrs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gubznocpx.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gpchgyzvl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gsxeeprym.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmltzzkcu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gqtryiquf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/gaxspcuzc.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gqdussvle.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gsoowwndd.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gzhsgojab.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ghnnosytf.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gwtrunazl.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/glwbohfpn.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/glnadbunu.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gaampspcm.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gnrcvgqyf.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gahumljnm.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gvzveslyn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gysxstiqe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gdzaexhxv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gjwapguib.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gfpmfdxsb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gxloaancj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gemomopdb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gvlhmoxdp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gftaxtlru.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gppfojcqd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gskpyucjn.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcsohuzoo.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ginhpcikp.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gysvcdwvs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gglbpaciu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/grmcktjed.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gblgebvjv.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gceptqwly.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/ggvnmeilf.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gdlbiybci.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gejzbgzei.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gdgotpzml.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gkmizulda.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/geblinxgu.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gcujamxky.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/guzycudbu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gyoyywxiu.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/ggjjfhdjq.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/ghvwqbfnz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gufuaiyxa.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gocxbbqwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gdrdyajpe.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gjmlnyqmg.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gtdyygamz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/glhqmpuad.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/grtuytwxw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gqltvfxxq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gadroxgck.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gbwyafswb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ghfspambr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gsvpbsjxc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gwmcewbsr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gvtgbanwt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gevdpwvdb.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/grfvcfzuy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/ggxvfayvn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/grzyouota.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gmiphljcv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/garcfupmy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gigytdbkl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/graqququo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gafkomzsc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gcyipsdft.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gpjuifgsu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/goyzxolhh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gyfkybmke.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gzznmxbgj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gdsivezso.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gozfyorln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/ggcccvkqy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gstpxfwhn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gibreggld.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/glrmbfaxu.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gqjubltxb.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gduqkrdkf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gedglwhtl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gmwrmodej.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/geudlrisu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gtnblllgl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpkrhbbbn.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/ggkgcidim.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gpeqhakuk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gzxiufmyy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gchijlhwb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gleyvtkru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gltvylpdb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjfnjboxo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gawjifpwo.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gnixtfkfk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gadupbeyq.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gnkuhmilw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gcqoqoaly.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gjnkvniyp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxjrwhmys.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gwuygpdxg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gkduzggmw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fehbvm.com/Article/details/gmpvsvlzl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gfxzkjjdb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaebzolnv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gsgnozpau.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gyuurjjub.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gmnvzxutj.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gqychefqi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gpsnxqysn.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gdelqrokl.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gnmuneyas.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gwenzkyex.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gyovdwqnk.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gqyjuytuu.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/godgoivfw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gvflsqbzc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gxarysttt.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gxugwttvm.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ggzoawpwz.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gnrrrnheu.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gprnopono.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gtcyfxwsq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/guucsrcih.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/ghcuujadi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gkjhmxmal.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gaeaguulb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/giqjiffct.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkxpusblx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gbtuguyee.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gefsrbwpv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/giwzlebap.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gxdfmpwub.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gcptikfuo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gkxtncels.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gqyihvtal.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/girtpmioa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gykmvmwcj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gcdnhweox.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gwdyyndaq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gmvkrxowb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glpahetzf.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/ggeyfdwod.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guwhrkfxe.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gnvvcnniq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gcrpfswes.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvuvspfwq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gvukvwiao.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvkkplooh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gmnytoyso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gxdlaoygi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbwgyfsqo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjqbxkixp.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/getyybnvp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gjmhkwbfx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gzcdxalmd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gcmmhrfee.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gcmudldxa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggzfllceb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/garsdegfp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gvdxonbuu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gvnexswpb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gurliazhj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gcekmconz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gtmvqowoz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gztppqddk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gemenocyu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gkrreijnm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gtumuctdh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gzmthgdpa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfjuhvzmc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gczyztpnc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/guqiqzdsa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/govdmbbyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gjcyroysi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/ggzagyuzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gymyvptun.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gqvlcjalw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gokuhklwu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gffplhleu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gjeiwebwx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gdjoomlyt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvskighrh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjoavlugt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glzqylwyv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqfljbwdh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gxjjldjys.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsfdnkmey.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsqqifpfr.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gdtspftzu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqxncshak.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwebxppuv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtmagsrbf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grdsmfjau.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/grsxcbkjs.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfabwgtjn.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbhamlqsv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbejfdjjg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/giyovfevt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gcludsyvo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gczhhdpsj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gcpqlxxqr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gqsvxrwlo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/goqmhazmb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gpvxridhk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gaiqvygjp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gknvqnuse.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gpewkwcvo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gkucgwvda.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gjpmhmban.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpckaigni.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjvytnesr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gqkcgyvpf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghrdayhys.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjgnpcstm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/grlwuzpmq.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/glzxntqpw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmbegkxue.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gaqrazqwe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gekgzueje.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gqnkzkwzz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/godmmkfkc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/giuomqhds.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwslazrbd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gexvrcecg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gdmkuzdgy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzmcussme.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfxxejjgy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/goqhrnrzf.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gofuaxdvw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gvouybjjm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gscbezulk.sHtML


<!-- 参考信息 -->