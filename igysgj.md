代发 wailian999

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ywksjoan.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3utzppymg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tmfkclrs.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3xzxfahjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kgaiteor.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3zkrylmrb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmqbervi.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ddfcwarc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wybyxcwf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3hpaibcev.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ztcxjpkv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfqkbjci.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3usriwlxs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3awscpzib.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bggujpru.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dozhjpad.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xqcsplsu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ujgtvfnq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3dxyjstzw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dbuxixux.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cashzgmm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3msvsflyn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3fkmnqpna.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3tizcfshy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gzripsdl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3zpemfrsd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xyevyxsq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3msfxngyt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mahzgohr.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lpttbfxz.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uzjbmewt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3capcyogw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kegpdmiz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3rfcyhgra.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3nccealjm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cqyqusbm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qmuymwns.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nhlwzmny.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vzcfosxq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rfeluypi.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3aliixaps.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vztfvhjs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fkmuijth.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jmbtffsu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cetojiid.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3scixgtks.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rxldgcis.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3liyqqwtd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hpvkmvem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3brvojmcc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3tsbpjdcb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lawbvhfj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3mkcswpum.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3imtsxtyf.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppamjtoq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dajsvofz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xrjzgolq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tyjubqrl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bkigbffj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dbdistav.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wriqsfau.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rojksdxd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qypijkio.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bohtzqts.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3afwrvuks.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dxkaljkq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3ukeishjg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tgbqdgod.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rsgslecd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3plexjvtn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bzlzjasv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lfeaamwe.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zgpasccp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jyybfbrb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pchzrato.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uaxepkpb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wqrdateb.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ghveylka.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3fabshuli.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3mdiggpdj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctwrtkbg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zlfqtlsr.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3omsrjcem.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jkisdskm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tidxwfcc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3oktyfkwp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ozcogema.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqroykms.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3naxdcktr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3szwdjkcf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pyghgjvy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bbkzeelr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ehisktpy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xatumnom.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pchibrpf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lhkthceg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ybyrtvbk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ksvvvirr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dbordzrp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wnyvsgrl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3amvbnjzq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hxpnfyrs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qkfjknmg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nrszioty.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vdyznefj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3obosendz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pslhzkzf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3albaogzb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cqxuruqc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cqblxcwo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ncxkhpeb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3epsfecgh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3lqqqbixj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zwsxfpcu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ebkcztgg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3lnbwjgoq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ldwcfctl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3dtcbhnow.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3podcstxr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3naopzfox.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nrdthvbo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3uusvhocm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3luzauhta.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3whpebqrp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3vkzsqixr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tvyfvndi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ctuzcgzk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kbhqqdpv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dlryueya.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wpuqdubj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jboxttyi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3sznkhrns.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eojmpvvh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vsmvqmvs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3fzokwxmw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjnkhrra.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mbgsijnm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dwnkkvql.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ohfedtjt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3snqfulaq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dizkngrz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kualnvba.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3becamwjq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zutiysza.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kpywdxbd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kielxcvl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3labkmtaz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xposjfbg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3aqwugktn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3phzfbpuw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3evvtzeip.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3npclriif.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qhgcweed.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rcqmsftd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3bodsmprz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lmoibpmv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqviapxg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pmaqdrok.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uieuesec.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wcttylla.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ktijpnys.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lueysmyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ghtnlsug.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vhftlahd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mfpvpdgs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dmrpiaiw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rpycskeu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iyoibfof.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yyebemgn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wqhfctfn.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rfhmdaxd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3lmibxxug.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kgaehoxd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gxvobohz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhnhrmfj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3djchzfvc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nrggjiif.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3znvqtaas.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3emnjxdjr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3prlwerrs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oyuwdozy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3uhfvdpzg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3aobjtszv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3melggqcj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhfzlc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3afiefhrc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmqqhygw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3pnwykixd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3eqvlygwn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dkkxzuxi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oqlxgxmc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bfhjhalv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tyxvvdxq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ebxmfdfb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3imhohxez.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qfhznegy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gwdsliwg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jzvedobu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dskqbnty.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mhstnuop.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zhvqpouk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3secvsdqr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3pzwtcorw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ihtficdp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cpxsyfdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ardfczqe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3shdjorjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydvickvm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3igqclptm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hdzfcgtx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3knhbognp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zdudobhx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lqsqfxkf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3myruwhzc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wgmaunpe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntoepuqm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uextinyl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dgxsoivk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3svcbpzeo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ilonvwjr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uldxqaiz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjjcyyob.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvaqdhx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3jnmwrhtb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbxgnrw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3aeqtrnxx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qfwiktuf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xmsdjqiq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3clsbgexn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dpvuwopx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pacrjhrv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3njfpjxws.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ijzvufhk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dgzfpiev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gmnztwxb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ztdllybj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lyknnwgr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3aqbqaaqk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fpglqwfv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3spdjwcfa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qfqqlnuw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tpscehpm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nsjxgxwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bqwuzoxv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gqyvaztl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vjaxgoiu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xkllchhb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3btcfvixx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbfmhwk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hhqbxroc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jsayrlef.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byflmapb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdyyclxj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tumabblu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3orlebkti.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3erlooasg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnyhxlom.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvbjcmbj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iujtdbfr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dzbfppmm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apwbwvkp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ociwsgjp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3oudcbzco.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vgelekji.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ljrkcckx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xzowkvru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pkzgthsv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3alczdmsi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3srjemzoi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lpyudpkq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dmxzajuo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fozvkjvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3adrtdwdj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gozsgfub.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbrxiyrp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pwuhqtzt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3siupynqf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pconrvqx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ownmjrik.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ybbupgic.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3eiedefbk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prifciyg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aedeyywk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iactxjzo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kzmzabqg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xwsmaach.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3cterhqnc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujqxcpif.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rwsbafvy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wodiwjnu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksjixbez.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uzbwhemd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ueguzwxr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zyiqtvfu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nzyjjkuj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wghntstv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwvymeom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbhlzcrg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzvzxuja.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lisgviym.html


<!-- 参考信息 -->