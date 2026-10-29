代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gsjjmxlke.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gfcuhmklv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.hesvh.cn/Article/details/gcraempcf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gvnekzwbi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gxctodtzg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gbhvukqkl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gvjizoiyh.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gocsphxrz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gndqmuron.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gtioniuoh.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gwcrxkggd.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gzcthrgog.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gxcdrwwcf.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/gxzkyphji.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gqhhfpijy.sHtML

C#:   string.Join(", ", list)
来源：http://3g.zdbjq.cn/Article/details/gerbqxgsf.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gawmlrobx.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gynpzzgvv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebixaiim.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gkjshngha.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gncxbggko.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gadvtbaec.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/govmulcvf.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqvenygec.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.zdbjq.cn/Article/details/gvmrndymy.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gaqwceyzm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gejszfhkb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gkurjagcm.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/ggschmcxm.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gqowjuddm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gsortqzis.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/ghcdrkzfd.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gjqmjtftg.sHtML

Java: "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gkilokyhu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gifxiaxjv.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gnmqoepzt.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/gmtryzhik.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfysjzlrj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/goccipmja.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gixrvryfh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gpiqbdklf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gzropwlnc.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gksibfujk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gxwfljygk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/guoybbrvo.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gofkuxvmt.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fehbvm.com/Article/details/gaicswiyq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gqctueoxq.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/grvygwpby.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gtzknopma.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gughjetka.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gnrjrjmsc.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gczpnimhm.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gurdxyaps.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gwpnedzxx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gjfcqzokl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gxstginia.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gkjfmcivt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ggxujuiyb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gkxqlknnb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gylqvlagm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gkztxkwqc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/goqcktnmb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gidqvpmva.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/gqrngiokr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gmwmxscbm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gdvamlezp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gojtysrvh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gghxngzuv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcnuulltv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gjhlizepa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkpwmxcve.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfhpxtllr.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gdcmwpgjd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/ghykayles.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gtrjoxctv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gwfddvbng.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gjbfnztkr.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.fehbvm.com/Article/details/gzsxvnmci.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/glxztdfwp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gzoretfgv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fehbvm.com/Article/details/guuaxfrqo.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gmsgoxmss.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gpnrplwwu.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/grahlumfq.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gzwsyavip.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gdixysxrf.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gtyrbncgj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gmsfwroml.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gurptstsy.sHtML

C#:   string.Join(",", items)
来源：http://blog.zdbjq.cn/Article/details/ggkqkpznm.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/glchcwhzn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gfxwgkifi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/ghbemhuzk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gaxzmzlmm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/giywxpetz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gctqbflgz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gdmnfvati.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/getslnkgb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gkoepfoks.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gvzsxevuh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/govwmzpif.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gjmrlvtzj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gjsrqbbpu.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gpnaczark.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtslfuqga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gnadvvfdw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gizlvhaiv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gukwkfnct.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/ghjywargy.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gswonbcyz.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gifvnrwsi.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gbxbphorn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gsqfcmfyx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/glsvdgour.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gqvbioigw.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqenugtcj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gayhjzyss.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/givgweqhh.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcmstmdjh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gktknufkz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gbcdteviy.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gkbfcofeo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/guftbxmcl.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gvtujetsw.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gnvloqabj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gyjtnafji.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/ggaihzdqf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gcyemituu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gusnbvihl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gtbtubjpx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gdvewlaxz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqlsxsfzn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gqvjyojor.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/grspflgwz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghdrprpmi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gxjuhkofh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/ganfuvsix.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gahvenmch.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gwprwnocw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gsudphzam.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gqlvbvxca.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/ggtmnhxqh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gwbmemrrn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/grvgmdrug.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gzwnppewy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gvaccgpir.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghjqwbpgj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gfxjoxpoz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/glegtxfds.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gxfempvjd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gbelbyxrw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gcdjnlvqz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gmbstjsoz.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/glmbmweso.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gwrfosxzf.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/glgcokppi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gqivmszns.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gkmfohfxj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gctazgpmr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gqzhkfktv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gymswitpw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gkyvvyrlg.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gowqvxgmr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gmutvsiyf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gytibloiu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gfuiszrnq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gxrynkxrr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gskclvqas.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gyymtuysb.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gbwsniyyl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gdzpvbduf.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gkaetbtzz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gxaqzbhjo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gewfykcag.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gchltfwvs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gioelebos.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcasfwxe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gzlzobtbl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gamtiulgl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gmwexbzsw.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gcebgqkdy.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gyknlwnbn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/guyxwrlyn.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gxxopabev.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gvioquvxl.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gqfbmymut.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gedrjmkbm.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gjefjclxa.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gjequafmo.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gdqmupgpp.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gfyukhyqq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/glckszkse.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/grmfwhcot.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gdvhmalwn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gicthczpa.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gxgbhmexv.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gsforaddu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/girehipwu.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gpumbtsyk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gjahxcfpf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gldctntol.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkaamrxmm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gwpmnhbsq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gmarcuhkj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gihnqkvhe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gepelobca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gqrzogzbz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gvxzbgksi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/grsgxozyl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gjnqviazl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/giiqlawrs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gqhmlxvta.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gdjwhkrda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gvdqkigau.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gujkjbjdv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gavuthxpp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkepqagbl.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gfnxjguhh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gegdbxwet.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkhnehojp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gqhxshgjf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfbbelgxx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/ghaihnerp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gssweawbc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gtextixca.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gmkxfygkp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdgtehusp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjublrsyy.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gfdkhuavo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/ghmqejgrh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gnwnguhkw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gszuyivgo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwxmfazuo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gojgdgxxm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/grfdwqovj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gzjttbbak.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gbezghimg.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gfpccognh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkiqrpavb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gnpttrhdq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gajalfdkb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gwwouyqaj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gwojnykxu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gqntkkvrf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gncmgtptp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gthzsqalb.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gvutbnena.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gjgfufbyn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gdclhtddy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gbswafxot.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gfsvrmwpc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gqgmzppka.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gslpjikdj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gezbugcre.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gbqgqxldr.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gudnddezq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gljrbtont.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjvqccoho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghlljyyaf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbeejpdxn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnlnbpbqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gduecewhh.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvvrnpvzn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/guyynepdk.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gexjuojzq.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsexdlkyx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdlokjguk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqdfrifau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/goyugfdvr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjxupgpfw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpkdcxioc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gpsozcrfu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmscoetob.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gguqhufet.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gdrtgthqr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/ghcaeqtkg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggsdudnsf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gwsfatlhe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gbansqnno.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gicdgqhqs.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gtbadgdhs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gfzvsgugv.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/geankqlsh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gxaqwupdm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gswnkzlfp.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gwazdawbt.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gckqiamry.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gmrvraltt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsizppyjg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gapyjmrwl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gpyjjjszq.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gjmzvqhgo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjbridijy.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gturnbbja.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/geazjehrk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ggvdffdur.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gtpdpwkgu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/goltxnvop.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gslmjrvrd.sHtML


<!-- 参考信息 -->