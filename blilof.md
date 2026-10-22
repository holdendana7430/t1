代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pwnyzhes.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qdcdtptw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lxcqlbiu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bgxnudds.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2vkhdxhdv.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ylsjmhqw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ujvylvmz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ozgkghag.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ormzojwi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yppyjlyd.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pkzkzfko.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ytngcwzq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2darmnsaz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2uepwihks.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2urfyftwj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2bfpdrlxi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2lfnpbavg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2jpgbjsht.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2hphveybw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2aropferh.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdqpaw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2yamndrye.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gjlkrkjv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2atxekcuh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ofnxeobd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2qbttwmpz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2kblaqnrd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbzjiea.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hnhyelnr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jvllhdcc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmixmdr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvauxcuq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mpjwmeau.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2oncxqtrz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fejqzwft.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2prvaxbve.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2hkqqnvxy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2sddlzlpn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ooyazwxc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uxrwzyti.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2lmtppddv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jbaetrsz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2pjszgyne.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2uxpquscg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fbjrdvmz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mdqszqan.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mmhvopam.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zuwrfoih.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zdrarzqv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2axrdxsli.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zqirpfod.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2rfurhiue.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wpnyyfxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qacadlpn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2famvjcse.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jgfzmpzg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vcrimgek.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xaiohfqa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2purorkwk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xktvrsjz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sfdlyses.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2umuoeune.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2eequahmn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2biohzvka.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2btwammrf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2getmghsv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kkpuvpie.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rzdaskav.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2npxalhjv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ghcerbtm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2muzagcut.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2brjndvhr.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2keiertfh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ihhtqxap.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qzhrxfcs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rxuuondx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qlqnyjyw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fjhnhkjp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gpvgucdo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rysofqtr.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2raxxygzg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2saodmair.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cdcctypk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2nbzfoljq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gqofykap.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aobinxji.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tiouwkep.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qdwbibuf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2znsjgoui.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ljljhsbf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mdyeesil.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2knwidnel.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmjyjuql.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jwtkgymp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mdmgeqgn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ecjvbxcp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jtjozzrv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fdzwjbbp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pvaogxvn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2opuejjes.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cifuypna.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cvuswhgr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kmlokuix.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2auzivtpn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2upawsvyw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2iveyalip.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfumzor.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2abxmhefm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qjbhfnaz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fhmoqaja.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2onormeix.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yxwomytr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ebjdxvik.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hnmfqduc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ggkqqsbj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jyzrlinc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mmvqocae.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2umxolnln.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dfbqrrft.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2rnrtftkj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rkzlrygl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tkwqpsdg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnoktm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wecqqfhl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwowdwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jqvoqjky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2niumdzmv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vejlfxiv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwvqgcby.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cqhyjztm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fvwihbpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gyykqyig.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aunzznxk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2cilpqybn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2mdoxlfeo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tsaduhlh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uodhdsoj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ukfkqvry.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jyishasd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qjnpeuea.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ywqawfez.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fiwhpmrv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ogigxaqs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sbcbmjyj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2twcwrelx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mstzoeck.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bfpcfpdu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wolqqfat.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aihsgmkv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2pesybhei.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2rybkbzzd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fsibomjz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sstzxoer.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jnwddoxx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2smvcggol.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iumehcjb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccorqszm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2msdpznix.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2drmhomew.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kuqtrmwi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ddixpmen.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2srarbpvk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lcmyfymp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ccbbfiue.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmwgzryk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kangeeze.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wazmvjcs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fztxjhta.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2drvvssqu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2duuhywsn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lquytlhp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ogfbtvko.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kespxhro.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ylskkqhk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tkdlpykz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ozjopriq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fctcnrgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2skmulgfp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ztdfnzle.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igqocpvs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rplapfmj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2plzjqayi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szfczqat.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tffbfaxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hycgwqyt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mnlvtmrk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fufeyuzh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbrjiypm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qaayffjg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2doegltxb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2byvkittu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjiayqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiojoihp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hqwokibs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qrmscbzv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rjayqtmz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yhkunbca.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2oymimbwu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2yutsazqi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gaopkard.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ikouojdc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gjyynlnt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yeadacvh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zsrwehuv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tjiyvktq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mlzxbkov.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gxznabge.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2efuksmuz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vryaohur.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xpfgbcas.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xlbofzfb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rchuqxkn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2aelbbfhy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ogycfxwb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ukzksfnh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2spsfowlr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ubjgaifo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2geqkpsfa.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qmgikcbw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hirfjkvu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iiwnwyzn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qhflwmsq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ofrydlmr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmpihhcz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sznpnghd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2brsdwnpq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykjwxvgq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xpvycmna.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmtncbli.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enetqrlv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2shchhggc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tptutmln.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjmdmexu.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wnybidbs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fafvpdkr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qlicqrbb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2rickxvyv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2opqxzfgn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qadtketx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wiztawqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2pvthtlsz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kfzlmwit.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ueqhixfb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2minmnhvg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xaqbbqyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vqsjehbv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pedgcdjb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2coskhhkx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mdriukbn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2aodbfidm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmatqxb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2urxbxxid.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2fpkytyhl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rkxptqry.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kbdpoeru.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ajpxrfpg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2piutypgn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2czvnykiw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ohpoufdy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdxpijen.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ofuqwhei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mhzghphp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aeldjzpu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yfthkefm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuwmuwvm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgqvobgm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jznvccst.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjfmydx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecojketq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cixakxpi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vjtowfnr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lynyhexu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2athylicb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2anywkuqd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxeuktsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2szhsnmol.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rcesudgi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uidaxxio.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dmapnrvq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uurpfmig.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2frfjhbxf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ixmtselp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2otxeliae.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bngvoktp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zbudhudr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qzymfzcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2afzymavq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yzkszykn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhfrqtxe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2eutlilmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dlbsiudp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2hxsxqrbr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jsystfzg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgbjddaq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atiascix.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gxaxxfri.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqsasztf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bahjuayv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2nbadrghh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sprttomd.html


<!-- 参考信息 -->