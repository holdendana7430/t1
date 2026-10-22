代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ylztmpjb.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rgijrror.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2grhknjez.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kksmclay.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2svowdzzd.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2fdgupshi.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ohybnlqr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wfnxzank.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ndasfzxl.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nvrzyxme.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2uwkinsvv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2trvobasa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fslkyaib.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hvwchzub.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hykijaer.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lkgboous.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xgirwhif.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2azjhfjqc.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2sjptgscl.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bmacrexx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ehvygkqt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxdrbyh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2taaxjfcv.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2iiilftbh.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2jzmhumyu.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xcecsrku.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ccdcmxuk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wifdvazn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2qraawpfp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2oivmvfdq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2sffisxmq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqcjnrl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2pahuqvdg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2xjjctxmg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ccmosoih.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zukiaqrn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2wmggbffq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ngmpneyk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2giojmegs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ajmnejsq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uvilfyuv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jevytqvw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2lrtppdgk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nrwrwbjd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bvzalgct.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sjdlbllk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rfoviytn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2irmfymyz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qvwmptjq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2gydlmkwv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ndllftzx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjzktmg.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2jtmhhaar.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2fcxlijqm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zsyapidp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oevgpoip.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2zmwvhbve.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lacnxsjx.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jnsikmue.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pnnsjmlv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ewwvcezw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zbpwvedq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ttykfwkx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2gerpdzgw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdsadgo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2swsiouuu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uhkvvocg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wdesskad.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vmevvwef.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2jcrsqywc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qrqjakkd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikilhmkn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2hrkkirhi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xrhhttjj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpctwkj.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gfasnelv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ctkfciig.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rpvsmbpg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ktowiiiu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ndpmigic.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vvytswet.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kyosmwax.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wmqsnhqv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2bwsxnqyq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2swxbugsn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gcffmtgk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cecjyngv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hfmxwhro.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rrewwhsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rpilzclg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gbrzsioe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2pzagdwja.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hnnblpeo.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2arhoxxci.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rapsaowr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jzdyyacj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2hwpwoisy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wpevhihb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2vdaogagx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2thsqamen.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2upzfurvj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rziebahw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnssdjgr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2aginatsi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jjhiaruv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ynnavuyk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yeoldizn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wegowodh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2krhziyli.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2kwxloort.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ebrkfflf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tzkmbjdq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jvblpizd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2czxeveof.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mfeafcdw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rrjmyutz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2goeygkjn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wftljwyt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xbwogqiv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rouaoumk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uwqjoqkx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2diwessub.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2dnuudgwo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhnrkpim.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2yhnbxege.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kjvolyyg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2caxatygk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mubocoay.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2azivzgqi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rbevbdyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bzlymftu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gvtkaobu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2cnrctuwv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tepawtnn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ixyetgky.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rhkgutkn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jemgkcvb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2euuvdlco.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2offrbweu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrennkcq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2talorwqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2etrwtnwd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wunnamzp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lpezjzdy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbqxthfo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2trhbzhwd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rkbdearl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kwtdwfqp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzomkiho.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ykbtkdyy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2huswckgg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wdfvjuay.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2faloajlj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2seekahwy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2pcfcqwgr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hoelsqcc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mranmifj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bljfdmtr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2asikqhrl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gofzjegu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2frnebvra.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2oyccvjqq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2elribihw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qcvhoyxx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rktjiiqt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2gerahnip.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jazbaaal.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wfcbaxbm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rfzixllk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rqxnruug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnfufygs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zxgsozvt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dybxsfml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dpdjqatk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gvjchafq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnvrnegk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lzhxcevv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2knkukqpw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uolhpqol.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqbgkcsz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ixizfxfg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uyksjbde.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2llmiceiy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gnpzkjue.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2erqwbdrb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2aonltdgj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mdpxyrsh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lezkhedh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pvixtmsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynmsbbem.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ctwenusv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iiycfaft.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zyhubask.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2unuumthz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dscrvvij.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2berctsoy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2patkihap.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qlqpfioq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2couwleny.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mluwoizg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pvqxmiao.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdoeewrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2llpuykrl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwwfynzf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpxbqbju.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cqwfalnz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lcjqkurs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jdpxrrwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xsjhlcdm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2krkmapli.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hwfkcguk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2skozqmly.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xgqrefii.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hxlbwfau.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2quinypqn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bqshrfwf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rhzfnycu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2utvxwzzr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2teuquihh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2waazjyea.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gsdrrwte.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2mhnnnbno.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rnnnudhl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aithbxnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2qwuamgvh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2klxikggp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yuktbyys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2gegepxgg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zfhilfqo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kpwyprve.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iahfguow.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbsrlreq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gnbpftco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zbhzealy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yjrdncok.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcgrocfi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fmqtmsjm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zgjiycei.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dctiszgn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cxfbkbtf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iazudueu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzagghcf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2znkgnfib.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clsnsvic.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxsbeqkq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hriotzuu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2dqbfjnak.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zehnrkov.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2njgnfncg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2elnbdsrw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lpqxjglb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2diiqhgyl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vranupsn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xltklkta.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2poveprqw.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tljvjswm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ecvconwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2yzodccjd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zhhdvlhu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vejdqzhg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otpcvfhu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2btxzwyti.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ajyjquqm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kcnmzqdr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pbulbemo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oneglwpi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sluyehgi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zcmwndgy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jzyvvquz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2juudhbne.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zoytxgmp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2matkjeko.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yfurewnt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dbqgpnxv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqbnkigv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dhlavvzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itidegur.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgfffbgw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2owmtrzgp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uoizlsyw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jglcfakn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yudewvth.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yprkueri.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lftsnvrd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vnsxpqef.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqksgmtb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ngsieezv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddfexeki.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kgxhazzx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2osabtopz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2iouqwzin.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rvmstvdv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2sbazmvwp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vmteoabo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gxbkzgnl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gicctvde.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nyoyezqg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uzqztsrt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yszxrdwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2adtlfvpt.html


<!-- 参考信息 -->