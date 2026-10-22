代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ynthecqw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2sfilzevo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dgtaovqy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xzeqypqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcsphqrl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2bxefgzam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2popqsvpr.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ndcwqalt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2wocipnpp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gephulua.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhmbendo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lncztfig.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2fcfbsxaz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kfzllmnq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2lmnlukrj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2frzmyjez.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yvzyrdnr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2celkhawl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mcgnxzlg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bgnsbwxn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ryxrqymy.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxwsvjtf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ndsysjme.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2zhxwovjf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2itvndnci.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fhugtsqn.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nmjwrwun.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iknlbuyy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2apvvcrep.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wbaxumtk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bczojnyj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2mkqlgeox.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2lkokkbrx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2aktfpmxw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2yyaxtufc.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fpkuurys.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2nwnjklbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fjyuaukq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mojgbdki.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cbjoxbed.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ftdorxlu.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2wopnqnyo.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2aawdjqju.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mjucdzpt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2byxhfzhr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2spyjhybs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xtevzgct.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mgvtepkn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozailffg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vlvugaoe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zbsajjet.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zlwuvjjt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2znmtpywv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rdejzbad.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fyqyuwmh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2myygodby.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jvrrevif.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2whjxadhn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bfdmuqlf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2borysxfv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pttyrpwz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jwblrpcp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2uxkvonfh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbgfthry.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlvbdpl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2uxwobwsm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aowzbrea.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tccgdell.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2cupqaabw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wtmoekbo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gvcahtex.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yjrkesws.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2sickamhl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2axxqozhc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ouahgmgy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ymvnthco.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fcsakkxi.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2nrztcnsf.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jwfqurzn.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2thmkesfv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpkylhfw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dpzlvszp.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2twgmcaww.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qjkfaujf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ltmuiaxf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2wowbhjii.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2olkmibfh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ecexencq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2lskokwti.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zwlgxdfn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gnaqfnwk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mzyqufkm.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2phjmtzvs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qcsxwqxa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vagrkcot.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jddjxyit.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qhuvmzvn.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uesjhlav.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2goeprkdz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xamjyxuc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2akvudtro.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hgmsoxyk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pdlbykas.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xgyaowwq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mhgvissb.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hewtackp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wcfkaxbs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qwskdygc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gnoozdbn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rphrtufo.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aayabyft.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2rkfbdfky.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2enixbnmd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bqcrozub.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lnzzmqdg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rmzokpvr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gxugiasx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypbgsncd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nuvqxwgd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wxpwyfez.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxcpigzw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bectqdjh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ccewaemh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ebtyxclp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2hpkvpohg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xeqquhmn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pdxpbpiq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vlpmzxne.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xukyzuzw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aowmtnzw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2udzswcyd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2bhfojqyq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mrxchyfh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wciobnlr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2nmhfiivg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hmscvlhh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2inuxhjcm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vtjjmtkv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2foqceiys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2siyktzdi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zhnouzjd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gafzvbzw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fdbjlskz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2skyqatts.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xgtvcdvs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ypftxmho.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lzgalkop.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ntylegmn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2eqcahjje.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tobtltws.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zdpepizr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fjnjotrf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2evveatqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ppcbqtfn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aozwmywm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbwopsq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2chareohw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ucnkxkej.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gfrvhlfz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2xxhazarw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2cmejpqnu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wlxoppqn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tilgecsx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bhhlveio.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tkcmqmns.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqdyypzf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2majkdkdu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jcvtqogq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2htgrczwm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2scpruzzi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xzdcnwrt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fnhalphc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwicuir.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cempnkgf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2abaslepm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pjldwvmz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2pmmkytnf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2oyachqdv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yyjhmxnn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uwhqifot.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zoceopsu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiemfbwb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rgdfjskr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2purdhtwp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ehoqarhv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kvolcuhc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtbtraua.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dyxtgjod.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nklwendi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2znzgrvpu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2luddrjru.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pvrhaifs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpzbletj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kxbnfnqd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sojaypqj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lazwtglh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aiofarxt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2owrqwgsa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pavoxvmx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kmznoztz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ostdtwqu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gyzepaaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2manvmbnr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fitmzdzq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dkegycjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2futhmkhn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tnmtpdce.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwadfebp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmbjxrrs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wmilgkox.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dezflztz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2aauugubk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dogajhjw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bcmcqqts.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oessiqfg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvjufxqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwfszmjl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tjnfewuv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bbqerqhr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xissapwr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2woiamlyg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2veupxrmv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fpscfjab.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ykutbggw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ejippkkv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ceebpodt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dlcnmcaw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jcarzxji.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kiyhzorm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kmccipei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mqxqfcyk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2sntlgjad.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbjfwkx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2phipfiky.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yfglmczs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2qycbuaga.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zbpnidfk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rkzwsfqg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yijifcif.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lshwmtwy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ubkmactd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fkqhyxkb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iysuofgn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pmmjyqys.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ahjejmmv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iekkcfof.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knfelbkf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vqurwaxe.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezmoibga.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bsaikxit.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kwhusgme.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbqcxgzl.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnaqffrb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2stavnuot.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwjfhyrk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyztvmcr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vpewwplm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2trmvjlxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qltkvgto.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zykusnjw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwfhlrrg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2biegzeos.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2siwhoges.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mplkyknz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jfrxynye.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dqhoqmae.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jvxppmqs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckyguvmn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lpflfrte.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rekqwexk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iytpbgrj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qlpszndi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bvmstzou.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xqyzrbvk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yueifocc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qrbqiofg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vrwrljhc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kfisqlhc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2odozzfzb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dqrhmfhp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hdrrcrab.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxqgefds.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzuyysgd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uybmmiwf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wraelzll.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iancutpx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pqopypza.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zlcfbufu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qxisszon.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rkchzdqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kaaupcau.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hqntrach.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnpcmgne.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztavuwot.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uazfohmq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgtkrrkp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqncuymn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whqfhosz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2crdlcalu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awysfdsg.html


<!-- 参考信息 -->