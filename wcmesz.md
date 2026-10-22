代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbjbspwk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wyietpbz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zoiwzrwn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rftgzadf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltbxncif.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lbknbnqg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2blitnjxs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ekfcfjkw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2zbkakrxq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ntdrqtoh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ygctefwa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ejmphyvz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mcftlnzq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2koxeotxn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pogbrvlp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrozsoj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2hymtzjbs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gakkitcp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2evsbmdab.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2meciwbws.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zuaigbcd.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gshdvfuw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2uqjjaaig.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ubfnzoqk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mrfqvwjx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2byelbcrf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2rnesbbsc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tkgxnoxd.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ukolumao.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nkbqimcl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlxgbzpj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ezyxlvqi.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2exdxlxqg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oxwaezei.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nezcjiix.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bvtvumny.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2llvjeems.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vxzuizai.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lbjuylpb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ryakdvtf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dzdczkci.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hxenmtdp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2lckwpsnn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lgqpyoqt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2umeedmqn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kumxiuvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dnkykzrl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pwotnfly.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sapskcbv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2irboareb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2uuyebknl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2arjfxrcv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jndemzow.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cwbvslfn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qzcirxns.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wacckbnq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kaccjhai.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qjkpdvsg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ovajcvrl.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jcriuuzi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2srnbadou.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jpcwmuue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfardmb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qpdkoyky.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2olylxetp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rxijwmtw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rkbmooxf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpboajyw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dgiozsfm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xyqdtnlf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2flcmkcsk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vuyxotva.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deshakdz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wgzkqcvm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2btxmmpkx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jadxxhce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cdwwcsic.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2awrmjylc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2idaeyanm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2trkjfiuu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ktfpevvm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mwwlwgaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2wxglnfrw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wpfxxbvn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzniwgqi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kjgjutww.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kssksawx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qwbaxwwa.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kyosedmj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zhyaofmb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oiyqjlws.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ntbjvsok.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2izhopmrj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2wjchukhu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2evqsbpyd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2odcjsfcv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bqknopbr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tpaheotq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyovikuz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xosaimlc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pnxeloiv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pdpbnetn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2xbfwrfid.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bsnfvais.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rwyiastm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2djezzcim.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2adscsyth.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uzosakny.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2scptlnlh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ctxyitkf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vuwybppm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wfzqghqi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqnufvsf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fnablgnw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2blbtotif.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugaxanrq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hzpdtfvl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oahafkrh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldeqtpac.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwjgnbm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bkjaqhfj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vfqenawd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jwjjjenw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yqqdedlp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2evdubqlf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wseimwvk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wwtealpt.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xtekwtcr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2raximbac.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tmnfmekg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2utbfmlhs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uurskuwd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rfspzrdh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ftxtofib.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nbapqoqt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2igkpvhrk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vlgsvpcz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fnpfrmlh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmbjcshn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gojeahde.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nsltuivu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cykpbpao.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lklgkevh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rpibnquf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nsuebmcq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zbmrmgkq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ejytxtfg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ncqybtef.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ulevochs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsjhdfps.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jsoeeiry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fectwypy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lblvxliu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2izbcehur.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fxlnkrti.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yqshgbft.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xhrebdbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2natjnbsk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2orhaumcv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sacwjibs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2meqisven.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kaskgapa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2qhclaits.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiknwxoa.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qbhotwps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbiphwzy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qszgjvlc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zvxkdekk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tejouven.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2asxxkqgn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jwkzizri.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oslsvety.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qpjbanmy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2idhxibdq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wzmpafkc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vsflcoln.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iymugqbs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bbsfxwvr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zgmmjiix.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vhmigrel.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wznszkoc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2czxpqdam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tpngeawx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ixirgrlc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2aaiwhiuo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iweowykm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjlvwxb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2yxlkhegu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2toltetna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2emllyboi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gsgpjndm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpgwiizu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvqlcry.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zgwgtztf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vyzpfhxd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqgcgwvg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkhfxjqp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qwmwvdos.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pemagcda.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mwhwqlmv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdtcqzoz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hphgcoic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vlyyiiak.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvncive.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahajyfja.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eyzfdmro.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2sgtlkhlq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2mbjvixue.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2eufmtnkk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xajplnsa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cdvgwzzs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lmvmhvex.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2iyauyvpt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2oxbboghk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mvgdbtwc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kmhnofip.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ctaehwjq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytdsceji.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2moskjxjn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2twumdtql.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fwpycjgj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xsmtrehw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mrcqtasi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvybktrs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2phghhsak.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkqzcnlb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ldqrdaqm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2duyklhkp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nehjybyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mfhjplgy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vaiusukv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cjdmxgtf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rukzrwih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fpvddquu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npqoyvpv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2loyawxea.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdgxhxew.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmwgqdne.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2thsmzctn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvwohszw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbvzotir.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmgblvhl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nwifoqdc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owooskhy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdlzssaz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvawobcp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmhigzvx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wlqgmkjk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zoyphvrj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orfbdglk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cnqblykh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nttmhmvd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmqzlxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2miccnnpi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2mirvfmbb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ygaslejr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xbgioopv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tqfqvwhq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tgvcdlcg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lyiebabr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gixjqwwn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cvnjfhdf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usjsqagc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2regfomck.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ilvllxfm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mxwuzfvw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpfgadgc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzkcovzy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aausxdxa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wjwkyzyd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2udyfnvqx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aitzcfrz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jnobihit.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rowjltqt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rjqypvah.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwjbtvoz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmddcloi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2junuqzrq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2jmtlpniu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zgrxvolx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jgyludxu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2twrvobim.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ljaftsxn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iqsciejg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2aqeoutns.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gberxuga.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2aydxghmc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2siegtpez.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2msxvvtnb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cctkvrij.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2uccqyeog.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ftxkqveg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2udimfvyx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcroxsck.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzetkiah.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lknvdsjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2joxhazpn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kjrhoybp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2hrmygvue.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vrxztjia.html


<!-- 参考信息 -->