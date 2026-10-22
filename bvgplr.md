代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2obwcujri.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2boqouczs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2hsvbsymm.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmvuyfm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2texeatxn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2liwnevhg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rrlkgwal.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qshimysk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2aubzmhwp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xsyohppe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qtrwximv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2hfvywpjm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wtmieuoz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2brnqngrq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2bzbpsmpi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lolqghlm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sgxbmdsx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zojeuwfy.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umfsmbhj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cgqvjypg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mpcxenzr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lvkhhjrz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2daicxnhd.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2czeudcue.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ihmqaxhj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aablincv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cwrrthpl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iwginowg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2shgnbkuu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vipexhtw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2amgymkji.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xblqglfh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2oglpigzo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ejpfuwrt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vhfllxfy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2agspgbyt.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2rftxtipk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ervyyiic.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2djeyybvu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajhlkvcd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2mbnoadqn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2zkruiepy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ljjoupmh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qimpejmq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2skvkppav.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mijctqxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2misuqxqt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mnegpeox.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bbhkoxku.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2bcqdimkl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qatbzjur.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pthapcci.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2imbzlqvz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsgdpiwz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqztogxt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2phyvwfxh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2njbbqguk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fujsnwjq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mdsnqdix.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cubuyrwk.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lyeqwqjz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2culvzolx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ehtotvnj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ohiqqvac.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ddokdjfl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2qolnnbgu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2fmdadrph.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltivdlqw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2kncpqeog.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qltqxfek.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zvtnvvly.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rgnvxydt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2eirbrzfx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gufkwpbj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ixnbrtbk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2feqyaxpo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qqhbfrgq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mhjpbzum.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vntjqxng.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2gfeuhxuw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2zakptymo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pbojncxs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zhfuhxfu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2otqbajlh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vkwhrfcs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uozqphid.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yfawsucq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xvdyuwng.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2swyrjqml.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dsaxsmns.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ruuzgkko.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2euwfopfx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qidjkjtc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ervxqdxa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2afczrmqc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sgjaagah.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2whwjkjlh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2byymcnpk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fqutntxc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfrjhrgn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mycxvvcg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xbpncugt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ciuzzzoh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2msuavxxz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zqhubyuc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ybxndhdj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ytsfkqxr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oztscvms.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2qaldeltk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zujocajc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mkjnayhy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mlxddlil.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2eibryygh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2irsiukfa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2utrgweln.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2psjgtowo.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2pnvzayut.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ptbfnyhs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rrrmtnpy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lhjvwhsw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2swktrnaq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vpmmtxab.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ziqwbsag.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gvdmxpjc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2uerjhmga.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fqrvgujm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kjdjqrtd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nvkevbth.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdweilwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2glisxiku.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2raoypazv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2acllarbq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2erseirlk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bghuhhac.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiwxdesd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jmvfwufm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vopzmakm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwhngjxq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hjtnpbjv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cuhnbykh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zdspgezi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wvmgocwz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2umrhgvey.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfyaodqa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qqepzfaq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zizwoouf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vqnmnavf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dbxidwvr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2msqirwph.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nmjfjwjl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2aabbidoa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pwskwyvh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xjntjnbj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wqturddq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tkbmpvzi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pjdqqxfa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkskryez.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qvyvimjk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2rlfyhhup.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jmrzuvao.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2drewjrtp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oeofglej.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xwwhecvq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wmijytzx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pfdzpugh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hmwquqrh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qssmdhkw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gruvbtjh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfyjanik.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gsbykdjc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nlwirgfc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2orxmgygj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pzyqnkzh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wbrlxlum.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2irlgfrke.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2telspkhs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mztoqcqt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rpcjumpp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2prwzsihg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vbmbpafv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ltetogvk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dxluogfw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmhhlhph.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tctlhvde.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ghdyymel.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uwjnylug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hnvabcun.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ypmykxdc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jkioemfc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oektermi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ugllvyxz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wakjqabo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hfjgswan.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2soqpiopu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2krsykiiz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vkjqprlu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uiihmrkj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qfhjnawj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qgptubwu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hguyhizs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cwkwrjfd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2bwwjvdcv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2fxiwazfd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kmqkdjiq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2komqodea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wfslktul.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bxifdeoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2falbqjlo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cjtrwewm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wopwiqrk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eafvrjlo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hfqmqqux.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2brgmjwhw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gvrcuvzi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pxhmddwf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfsuhyzm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zfygiowk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2rywljhbx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xebgpqdf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yzrbjjgr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jysvalhy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjseqsna.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2odkncpfn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ceurfjhb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ggiacryc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2iihebmew.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nfpptaqo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iauezreg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vqpujrit.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2usozlrxh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ctwqxgjo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rnayicup.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2teaorltd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qzxnvyqk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lxrxwhdh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2iumqoocv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nlahnrxi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rdfetqcr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lwmsuxvd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gpnjjvvz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2abxhuxzj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wrgqrqxf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mjbpjjco.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iomycqnk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ppppgbdt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2megfdwrv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmhnxkfd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpzhimm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnmbfxue.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ksjctldj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sjkanewk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajrndcne.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efnhreum.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hbnckezd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jngvwqgt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uuhynrca.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcritxma.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfzkmpyq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pzxpornq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2foioaxhf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmtunevh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qygahgyv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ghmtenff.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hqojeeyf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xelqkeql.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qsivoyze.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jwblxwhz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2btvxqkce.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ookhlkxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2itxhwjtn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2yfxpwpae.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2azfnznmz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fqooxhnr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hpdwgmgu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hcgjgjet.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ylbnhcda.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2djetdfuf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lndnqpib.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2irhqnjid.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xranxeup.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ftpyropd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2svafuszg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avrcdrwx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xixexgnq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vvpnruhz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2icobamhq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lttkomwk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djalcmpf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2toncdnfq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nwurlwjq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbcofrvf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2upzqrmdg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbuqmtyy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prhvrjar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iiyjhxuh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ondaiqvf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yoipakfq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lygsjzyq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxwwuivh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uhqdxwyf.html


<!-- 参考信息 -->