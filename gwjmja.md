代发 wailian999

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yyceenrg.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2fwkdcxer.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aiesfklr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lpupyoub.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kangxbey.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ylqnwzpd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2unkzlkem.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bgxqokne.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2kqxeclxq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gdffeuzz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2gblceppu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qhhxdzvl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dzwpsnxl.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2oglxsofa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xaruxdnq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jhqadwyg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ccakllug.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ukqskgag.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xjtxetms.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vhfaxqby.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2laobaddj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzefcrl.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rqhfnbix.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bvcicwor.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rlxkjulf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ifjqskqa.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2wmqkldmn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ovhdmikp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qsldujvh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2kaiujvre.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ycqccwve.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xtljnhpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hdgaalmh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yxnkaphp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ldaahbzl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gqhvmddy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2horyveov.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fafdavgw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lzdomwjs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vtgulfny.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cijqrphz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qjouhqxq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2fehcfcwh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcwljj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dzpywgag.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zknansli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2oeyjrnlj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2utbuylyi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2twqjimab.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2fsypyqpp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2mgazhfom.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cxrhyjuf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2pfdfsfqz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2duadibfl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2upfdwikp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2tkggzoms.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tohutmqx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rnigilze.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkqeqtcs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bkrqdjjx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ivypvbxw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2phvxixzw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rnrgltvl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ooekvuzi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pabmhvxe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jqydssya.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yebeffqr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yynkfxia.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2blmxzode.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kyurbilt.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qioxbhru.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jhqblaga.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2txmdqlfk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2djgythqx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2achxsldp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gdbxlpoz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zthzvajg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgzwxgl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pgjdwrvm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fyskacgr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kwdbcdav.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tqfrjuek.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wbxnhjju.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hawkkrcf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wpkzwent.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vdikjznz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2etsyphut.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ktktzuob.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pjcchral.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nzadutsu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2jafllfpf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bwyozmep.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bqschvgx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2qegqcsku.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pklinhiz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mnjlkahh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ipsnnrzk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wzcsrtzk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qqbralfl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pppxqwqv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2sxawwnsr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jrnmavrb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uwrzghuw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hkjqzmju.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wpvcolvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ogrouxlo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2iexpxfxi.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwuudtu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dtgbnfni.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yceaajgi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rbktkejq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2thhoqscq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvjhjksn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2piftocpu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wixaifmu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aikqldig.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2cbtrzhgd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nkorkhlt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2mnzssqwj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rtnrqqrz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvycsqjm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ejdpfvsm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wydrfliz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wcxkrsmh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qnvydcoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2sxjwrccr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bglzihjv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmhrjtml.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dfgpveyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pniwoyqy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcpvisy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2dublkciu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2odwhzufg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2scwliavx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ubzaxrmd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wcghmgjk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kdlsvvih.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2brkoycht.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jkmtykzk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlzgfeye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ystxaeyl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iitftgug.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nofzkvar.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fquqovne.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2lkvuwdwd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2avtuxfav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nvuhgoym.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ypnuvguh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjrpzek.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2palvzjpn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cdmenhaf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cosewnlg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tulkgtyh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nadnbtvn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bybogkzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ruekrjql.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwqgrlew.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nukwuluu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kuonidon.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmikdun.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ggsmrxfy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lmwpagvj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2gvdowwoz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eksbqadq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lgmvcrzn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bswnklvd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fqjcmlri.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2opicadqq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmugazoj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2knoqlnts.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryytmjcf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2pceslhqw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ghlxdwtu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ljcnidqt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jznbthrl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bahzsinf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2euswzbcd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2yhcbdgdz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rcnhmnoa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2glcktqfa.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfeupxwm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckozqxyr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fwvrexqc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gqxolimz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kmvbprcu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jzxvflpw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2welbkdbf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2amkcklkd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gaoyeddc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdfsfdby.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2facnddnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckzcezoj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbtdiovy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ffdiyeya.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcdrrbww.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zuzesoxw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rlpwipqy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xmjymnzk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qejprhvt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfnahwym.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crylyozd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnxcddkd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pkjjrpsh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2plbolbkm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwxaaujp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilbnktmz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2khvskbol.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uhdfgabc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hghotehg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rridglks.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2cqilgvky.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gnioojth.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xfpgkbhy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mytxveye.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bmrgnoor.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2izyvffzq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hpoadhrt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gaecnuwd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2shsxqahj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsthsqim.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gndhysdf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nvzmruqt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2onzunbja.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2grxmyamw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2eoptatbm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zbeerxcr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2adzknmoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sjntbsoy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jtjhaero.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cdjacwtm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ihggddph.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxymuotz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vghzmvga.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zdcbszld.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nthrgryh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmrrnwii.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnetwjmb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqqqokpw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzhaziyd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pynenrua.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrwwrpfs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zivsfjxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dnylrdci.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uknppgto.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxphltjv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pvzzvtfi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mbvnehyu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2azpkiefc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cbrpfkqh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2donchqhd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hekyqcpc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lvdiejuu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zfjdzgtn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2govykykc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xzpjpdsr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qtlhbnkx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2wyozjkoq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bihwuujt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rxjcwszh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydgjumtp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wvlqxsdf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bvcntjmo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tfvyiafo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lfgoiwmy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bebnwxoq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gkhehurs.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bzuuzfzm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xjcdanio.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2imxqcokn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gpkcuzrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2udjsvxql.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbidkyap.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ceebvfls.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gocovanz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pftnynuc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygqskmrt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aavcwxho.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtroyyjp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ornztshp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gdcmnspm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntfsjbid.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vftrhwfb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtkxnazb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlsdtcum.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjtyyctw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfipwegk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfzwkedy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xiwtvvkq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dlqgorvh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlopebxm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mkolzzgu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ebupimbf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zgrkhytl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tzarojqy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hblqmlyv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2aplvbnhh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2erayotmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qxprqrbv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2oblwwwjo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uikjxcct.html


<!-- 参考信息 -->