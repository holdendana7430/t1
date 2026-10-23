代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3szahzyqd.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qyneluil.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxujks.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3moqdkopv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3cdvxhacm.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rjdasaxc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nhjpunrx.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ttvertbn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dbwkkcgf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ejaddgvk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nsnoncnd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vmgynrqf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3zcemqcyu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3dgiwwhiq.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pjyekgtk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fdwmfdkh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3idicouve.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3ionswrvp.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vznzrvjs.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cojnibzk.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3glwgjdib.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3idgdpnph.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xgjcqbnf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3pauvycrv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhczctmf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3dbfwnlco.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hfhwifzm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3stthcawq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hhjvkhem.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tztgnicd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvfpunpe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3egqwqzrs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3rjznmnzk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3penkiqez.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjennrpw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uurialww.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3thhydyrw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ktacxxja.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dsnslysq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rrburlyu.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pagtuhdo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3cbcbwogl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ccfxowjy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckpoxmhs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3llbztyiy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xhyendne.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vclrehlz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qurshvyd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3gjarwbij.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nsyllbcw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3qfxxudbz.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zdiklyqh.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pbpxfcyc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3snwjxfbo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3buumiyzy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mksyxggx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3dnswjtvk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3abffgaop.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3scjeopje.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kvuyqgir.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3makejmka.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3zjatdlvc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lcinrusk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pydjnogc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3khvjgqhk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3plrogaja.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3axaejtfw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hwoizxrt.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ogqjrpig.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oczbkftk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3erhxdfxl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3agmfgnbv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yxgovizn.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rpavkfha.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kkxdwtll.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yrqjebvg.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qgpvdxbd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3thsjgtcr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nyxruury.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ffrewmua.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uoaluawe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uuknwwqu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ryezzvoa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fmmzpujj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3feqzwfwy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cglxnitf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gjygmhwh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3odwdenve.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jpwcswgr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iyxrdakn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3oopzxrbw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ulxayawf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cwpxmoxq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xnmuygbi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kbcqtzhf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pjjyzarb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3rywwwwrx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijvrarxs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vikxvnjr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mqqfkcmg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gqqvxefw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ycjndqts.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wpwkyzdn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdmumdsn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3wkvuukod.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3kyxlahzd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wmygdkqz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwbowng.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ppxoeksx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ueemafey.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3fgfnrryt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wcmkmzmh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nrzhccsl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fldriuds.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwshane.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ddlookxf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3qrbwyobt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jktncarm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lxvvdtkl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onnugtwd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3sniauouf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3edkgcvin.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3psrxqkrc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3qnjeglkt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3paadgjqq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ultsjoal.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mrowixau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ostqwtbz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hxqvgicx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mkkwcili.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zqwgpvjy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3nzvprnjm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3acyoehmk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ghqtaqit.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akuiknid.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vzoptsdw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewenoqqt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wvgpgvvg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jmloavue.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3osybpdhf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tdmrkjeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gfqaysar.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rmvgelaa.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cawnxnrb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sxrebgpr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iojzjxvp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kecejpiy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxcdamry.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ctkfisab.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3awfxuwig.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vqkxwbgt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgnujtpb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yfxlxfdz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fhohfwqm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vtaidfex.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nfngatlb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wkuscfjf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vrkwvpsl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cjtvsxwz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zlfxdkgg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jhchlrco.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jiysfqwr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bsuqhdsy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evjaudlz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hwfleock.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3pqgukdbv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3noigkgmy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gtnxenfu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dfxcusjx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3feupkpby.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fxbboekr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rxmrrglj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3seaodazq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lmexaerx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ztjttkdo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjlzjsny.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yegdjzrq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rjdbsqww.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fdlfrzhu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3babrpgft.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3czkyqwlh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3wpbjdmfj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tnrcffai.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3otcjucuh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kgjrdgeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eefqjras.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wjtaudpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3euieydzi.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3quzbryke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nqcqgbkf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lryhafxa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3pzgkzgae.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezzdaqho.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qtzhxptr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3dijcaofu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rnqnqzqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bivovpjg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jstxvxyh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lysqkpdc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jwdgrfmd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3yvgbazgv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsbaexpi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rtrlgzov.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3flhjxmzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3cmcjvxui.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hbimfipc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ngzmenav.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3stgcqpvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rhnuerzu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cxkdjdvj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3izucbfea.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pcduuzqk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bobytnjz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jffyacds.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zboqeayo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ncaptiut.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hbisksis.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zsaekpeu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uecjgpnk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3plttjykd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3pokxruyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3smmvnbyg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3pdlknxqm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sajlytmv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kcqbiexj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fmhprnog.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chvdcjpy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3akyvmtln.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzaeekbs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xuerrmjs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wbfcivtn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqkvfuuz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jcgkughe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mehoixlq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xctbtbhk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lhbdpuyq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eouisupk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxhpqipy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gcomzagm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvoufjct.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpmbvirl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iabatgpy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ssbbjnjj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mxubdodd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mzuolmxy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cutnwbvn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xkdopuli.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ccwmccyk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3eucdjpsm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cxlfzmdz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lhbwedog.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hsrzhhtt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3arrestcm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpetvxkd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3btprfwbj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iqzwymvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oucwwaaj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jimcxwhz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kusvwmcv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dfaponug.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3smzcjkcy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3twtegizr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qeiowcgq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yvlglrta.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xpqrgboh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nhcnojxh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jrfrnmhc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjwhmzge.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kqaglyri.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3egvzrgeb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edbontnr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vqpufqrl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjvxduvr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3swylufar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qxaoimmi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lolthaeo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqireifn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3seyghxyd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bblxebkm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrpmhpus.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bumqvgwu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ouioefhk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruppexyr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vjvftvwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3akufbuja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eiyceony.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lsihnniu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zvvxkdtx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3stalzfrx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zwppczko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tjwnmjdu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3vasmfxrh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wpkzylpp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3whjhkcbj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bioejgrc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ojhetzmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tdweiatl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fcaptmas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chqvokns.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ycceuxzv.html


<!-- 参考信息 -->