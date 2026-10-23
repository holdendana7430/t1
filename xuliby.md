代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ritgzvjs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3dipbqlnf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ccipskho.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tsfvwoak.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lhkqoupx.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3sjgzirvo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tdxasafm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3pbmmhacc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ahhvzzgz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3iwafdffk.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3dctdpqly.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3pcsnkvuf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3bzqruknd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3turpyfab.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zmjdpmcb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ypcakiik.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gsebvzyx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cgbgmjzc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nroadxxm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jkihmwtb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fernfctk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xzdtqisf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bglwvzio.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3homtapqe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3avsbeqsr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3dxiczjrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lmdoemas.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cqazrxtp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xmdzcdaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fbgsuvhc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3rjzrukvy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kzuqxeyp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3heipajxg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vkvxpxzs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fzmqoamk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jbwkorrr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tbdeprze.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3detleuui.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mhmsahyy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sxzaacxh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gobibzuu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wpqipbow.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3bwwdkvja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ycdzwafj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3iekefkqt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xpblwqmh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bdglinbc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fbzstjnn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jerhhcrj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxtaqoxu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3aibipfax.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ojbeqign.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrauarwe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3onwhmvli.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nlimqpfh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ncxqjysm.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3piqjehtp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkjdcnou.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3szkkxfzz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jghplwro.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yaumngdm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wduvyxei.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3hpenuuej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vnrnnqoy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tqmytbsm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ulzorlxx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qihbencr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bichcgbe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tzfrspmp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxrmokr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wwvjpyll.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3pgjabedq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vpaobfwa.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jzaonzqp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3jwvskzfo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uwslkdbo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zelytxgx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cfutpers.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bgxhgycd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3nzdpvspj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oqgkemew.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npvrsryk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rkxkupvk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uypsovsv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cdlnmkit.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ovrliyfx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ynxbrlyr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ahrecuyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rgryvehu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jpnxgifu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zkdjmalg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jojawskb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3myrjroie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ckrxmxwu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qmvtdwnf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cnjuazjs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wwvphrtm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ybowbqzp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3jnsymguj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hnqjwjfj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lgpprpll.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pewleodk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sfzenawj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yeptwoji.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fqkborpv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dtwhkhba.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wgbmginr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3htyzogqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3phhfpvod.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vbumrquq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kehwpwes.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nswdvppl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vfpvdxrx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eipxubth.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iebkwnyj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xzeyzgqb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mjgjkgnh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zvfycopu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zqclrdgh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ktorhgcs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jljecrjw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpvvcujg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3puwpdebc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdwlizia.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtepnjgb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qkorlbxh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edkxohzc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3toeerixm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vxsuzxmy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mdqshduf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vdvjrcqm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cymxqhja.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nykisacb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xldnyivn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nuuiqpue.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uwwhutrh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bhanukon.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3prfgxcpx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ykajmjil.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nmibqxnm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sctgfflt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wngqadeb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zfcfhuzf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3syoyuvwp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nxafieni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fejjkapf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bpixvymk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xlmjuzby.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3daraaaqd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3hqccmzev.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qaanqurv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mcawjhbn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mcfvtnff.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgkqpplq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mcpntzhj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mmmclxox.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkujcitw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3azlfwqzn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xodsvkuj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3snfwydqd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3vpohdkya.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgflxzhj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ajimdiwx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zidlktya.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gsjbxwif.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dsuwxvof.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3rxsqgkyg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qszjukjc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tbukobpo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3efpxfdhc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ytzjampt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vgijlstd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3smotblca.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3unzbnqul.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zqixeckm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3dskcunye.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3msdgyvxn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3mcdsdybi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vcvlxruo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wedjvbvg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ylifcouq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3idqmtirl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3couispuf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ymohxfez.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hhifulyp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xcyezehn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iwwewnkw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzulzkoh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyjvdmrw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tgapjcfh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zitzkeqz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gabqwkrv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtkauqhi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hjcchaju.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzaotxng.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3flcaezvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umrcrtso.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiwuiopc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mikpebtw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uimybaxs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbrmipzl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3apuxhwou.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3coxrftvk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pgzekbia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3txurvgme.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qhiwhkrb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tkgppnsc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3apugcqbw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cgzynvfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3kvzuctid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3azkygyis.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rsklcfdi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pwwhlnqw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kipazdjj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ivhlcuhc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gujzxebb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eavsdjra.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tfdlcalt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3zgdomftb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ndxqklce.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3babekxbb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ytxdbhol.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wfyeurav.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bsbndpgl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ypkrwujs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3khpubshu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tirikfyz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggfdchyb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gykpxdvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3submvsdg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okofwjqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpakpfwb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hngkcxdu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jetsgkci.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ieojhkts.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shktlwzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojeynnlk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxwofxsh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3oixjxmpt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxilejev.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tozzjzyg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aqaiqriz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3padkygpt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvbnqsz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wjsxaalj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ayvygymk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nhvrplwk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qwqkxmcm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3oxpxlcpo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hxmastch.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3neawkltp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3izurynop.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qnwnzbmo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3awdnczxb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kfqbvkim.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3glnzgisf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ermaehsu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3indgarrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lqksnptw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zpxwmbja.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dsoabtgj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3chtfgbds.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kvkropas.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufdrlzkp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzdvmajy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bribjmda.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oelncjyo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cjzpkoag.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fxjrjbxm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3pulqgjjb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xpftyfit.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zpfsaenr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aadfmini.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqswtmai.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rlocaoxj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bmzjtkff.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lriimqqs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3sonhlruo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3osvfihtz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3byuphczy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3llharfpq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ceqldfms.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3uwjnodwe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kpzuamik.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hrsdmvag.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzpwgfxq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vjncryjp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tkcgjuog.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcumuvjd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oskaxscy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qedicxji.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctfinchm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ejdnqzyh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3perjedai.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iamspnpp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3rnxisytc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3urxytemv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3caoyvmnd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pwxssvhv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sntxonyy.html


<!-- 参考信息 -->