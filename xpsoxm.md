代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2gjlchtvd.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tnajlmob.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2vzqkaupj.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2birnkeuk.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bcrqccvu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2awefpeqt.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2midavavv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rhhmvcff.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jsazpbqq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hhwhtprm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ohuyzjmj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uhuofssi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2prfwuali.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2gmicoxov.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ouhjukiy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2npnhhtzq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kzvsvxji.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dagpfxey.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tkjnhmla.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zdncgdlt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2gcvoubuh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zgvsxexr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2naptrdlh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cbsrgktm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2croibcum.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hnlhruey.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzedtfpk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jjafzlum.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tybellfl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jgvkhbvf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2rdditbci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2incjmzae.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrdgwki.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2jqieqelx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ecbcokhu.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zjsjtjus.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2heaflude.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2qczcfjzw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2vmlbrskv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2upewsdlr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2piopvxqq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ptoiofpf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2mguwxsgt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzcxefh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gjpivkuq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lsxjeivv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfshzmg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2avrbbqqu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmughhna.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2urevhsbd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cwojfyev.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sjaeczki.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sxbnjund.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bvxtkqot.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2krkcfvtk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mzawfowq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2vkagjsrd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jeofaoaw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qftwcyjb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ljtdvmtz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cvfiedof.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2bzpycxiy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dghtzhgc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxgbcok.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2yvypxofb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ojwbfwbn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2nfpsrmuu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lcwkhgoa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2cyuzwscb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ytezvqyu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fhucolws.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qgfmhexb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2khffzocj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gisxjbfj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2keukopqq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kchaewkc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2cigbzmsv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ivendlab.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ujceoemo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dwgqnnbq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lkyohxoq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dkmcpuki.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2isukuymw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mxszmwtj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2otxohowd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2epzomvnw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kixcwdlt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aaefnmvw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dflxouuq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ztxaeeha.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ohisjkki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qawomprq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xiujlbpv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2guctetzu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hbgzgwae.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wycrgfcg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhtgtzyo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qccalvny.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2cayeiqbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2yqkltkhg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tzzqnuuu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kjihnzcp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2acaisglt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jeshhfwt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vnxygyyr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bowzuvnn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dxxturdm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mulolrjq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jyjvnrkm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yyaaitgo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xinvcxmd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2gprnuwzt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dbbftpak.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yofbtatk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wmkdkccd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tqyenxdz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2owcyzpru.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fwlepojc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2avypchkm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2tslvvign.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ivyyrxrl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2escvhzgk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bzoxtmtc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vjjtqtxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ryuidgjb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sssfdbxs.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bptpqfsl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mzhxnhuk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hzvhobig.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2lsninwzc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vvjqifpc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnfcpgeh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dljsyiqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oealyskt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dpsdsczq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmwzebxh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2pueukbio.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vrmcgqkh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ymupjodr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2izoqgulj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mtcawxrp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gbisojds.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gwiqzjqq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jxlxdsat.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mvvrstkh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qtjflovx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gnfzmvqq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nsfhhayh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qbwekvgl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lknejhzf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qsjgzztx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cavomcbs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lnkyytbm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2iikcdxju.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ksaelswf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xhxhiuvm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2brwenlah.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mywnsmjl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tkdtohni.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qamcvhzl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vlqlawuo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2umxkeqgv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvnafmcg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ogoqmgmh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vhqqemir.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zqjwsapm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vcdegsbi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ltxetuus.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ijeobpei.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qauftofc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2gumbljyl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vcqtphej.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xecfstcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjyylmbr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rpswvygo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzkuuysm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hvymghck.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2afmnjvmg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptairnsx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2chtfoeib.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lonrrpgk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yljujgpy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ifchaicn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pynfzjez.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufayvujv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2foolitlg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2oetmzeno.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tuaawcba.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bmhnditr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vsfxpqor.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sjxllpeg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ttptsphz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ddotgwdt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2qcqiyhoi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nrlqygpp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2enzdraei.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ogspzdzz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iivvidhd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tltjdnae.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gjendtan.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bgzffzlm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ivqnxoie.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cfegegpb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfmwchea.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pmgqvppn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yujjomkq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ywzbboqj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kkcifvyb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2isodlgud.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ovtpjybf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2quewfaih.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tjnipufq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lyakjzcf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tlnrdcbg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2earxcayp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esqwhesj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvnuiyup.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vhkjcigx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gguuwhhg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcnjlfuo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iewgzhkr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfexjfdv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cijwllic.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pclcnoqg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dggtlymf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkzlvlea.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wahjiime.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sokrphhw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzmnjhqd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umrpnpiy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfdocygb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oalnjyjd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wftuaion.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2iqrnvqph.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cerknksb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qwaqsicu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tbetrmgd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wnfsxbmt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2etpnolko.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lilylvvs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kirhjtby.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2efxwnjie.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qphxksza.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wrvjdpqj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rrxxhans.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pfhhbgts.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2momlhdbk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2afpalgbn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2afhnhota.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxemyzbh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbiklbff.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kmountup.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rnwijozj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2psjefvvr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dujpbiys.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exyryjgn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2dubwzseo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nywjlurs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyadnvbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkhrussz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guqbllkl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgcgzkdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2weaqaups.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osforxgs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2emrnhazy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqoqdffy.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdpgcugn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oxddlmxx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2twglkhlj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwmoleql.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqmwkipr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijirvpfg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hnpbvnbf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfweurnc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kgipmkhq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nydlgqdy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2svfuoarn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zwiayupg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bsthrpeb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gwjixbst.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gjwvevpp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tpcrnqbv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gnplhvbk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gdrjdkqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugbmuian.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2svwowezo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2piroyrpe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2knomuvkk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dpomumrv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2cdqqjncp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xunytctq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmqqumob.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2emzvyzlq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xwqnhgnn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sxbbzkam.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vknubuxc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2aalmrbue.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qmqwwwvh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgdlsgry.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ahjqodjp.html


<!-- 参考信息 -->