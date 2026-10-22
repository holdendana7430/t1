代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rggfjfdd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2exfzuzky.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2sgfikvbd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2axyxlpuj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ikpzfoow.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bdiwciyh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ojfkyesp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2spvegmkd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2libemphd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2sfogcyrs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ppthscid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2benjcjaw.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2zcmlckbm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2cymqicdo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dldwozbg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2kbvwcugq.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vhoexmbb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yifoxxes.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yylbkdzb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2hxnjwiwk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2oiwkyqpi.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vksaoyvq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2uehkbhvr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2vdetyqsd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2znkusmoi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2dakbiufy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ljfuasgm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2aviztgut.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2itqbyokq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2pmbjidip.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2lhzralth.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xyjgczma.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2igyhyxfl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kbtfkizv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ctbiabgm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2godvfbnv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2amkwhjxw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2avqfkidn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nqzlbwqx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iubvgjks.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fabdzsaz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fyppgxcz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ctezufpy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jkfkjjpx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pwbacmzl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dgazgdks.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wnvoyllr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xjfcinsi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xmvtsrao.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xgkbunev.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hhewiuet.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aqsvcfdm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2urhqkrav.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sgjphwws.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ajaaivqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2nfkdgkzr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yxveebpc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aqujhyfc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tqedlbst.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ghqeuhbh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2rjhdysdf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqanoci.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqxmaupp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jttcyaqd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cckdzqhs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cbzjugmd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gmgygeil.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lyziuzit.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ublvvurb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fpxcuvad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adhqihyy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ipqpxnau.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxwxlsvl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2weeyjlqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rgkxkgil.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mrotdxfu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jygrmrjw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vmksfvpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ilppnyzj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2agywrwcn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jrkmgtco.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2eewuueyo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ukygkjcw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ltyvyolr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjskrhdi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xryojahe.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aulagodg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqxesufl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zmfmytbc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xgzkgore.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mukhuvsm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vhqwwgpp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lyojvcdw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixmuenjd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2afydriuc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ftsjnwxu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2aysdhuxi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ucvkqgvv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2smtpongm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zvunkpok.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kpnprdkx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hyhpowac.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ympftoov.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zioikjgp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2iksrwoxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rycyjtpa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fqaxptjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aztxhhwm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2akbnzzqa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mwfqymjx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2laedifub.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ubnunmce.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fqogsmex.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jppizebk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fcuvmjoc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oyxlxxcy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmkcbaz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxwpbdvi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iuoejvjt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rokqgjrq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bfokpytn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dngqqxtu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2patxuisk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fwoqxlms.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zxheonuz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vdvhqigh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hurwwsfz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2wtgmentv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bijxkbfc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2sawpmjkw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsnqgtir.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2uxkxkypz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhttej.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qoaqnwgq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bfuusujg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vtwmanxo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tdxbildd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ofueogio.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2databcsw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wsyvhpnu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zwhvqgau.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wmjysele.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rgmnvgju.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ovrmhyjh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qognwiis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zmcltdvh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zvoahwwd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2amtgqaod.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cbqrnivu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jnhilgft.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xhvqjdcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsfkhols.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2sadcfwet.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qkpsezmc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xukkjuif.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2avgyjtqo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2osevcdxz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hoytdozm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pbuqonuc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbhqvizp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdwaturf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgpnslop.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2riyqcwnt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqzmnqva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hfuqswze.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qzgemnvz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dyxcxujn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2drevxuze.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2owylupgr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufiorfzh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2llpfjiwq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vgadvmde.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sjadkmri.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2edijvdwe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrhcvnl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2oqouesjx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2advpdnib.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nzbcdfsx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mgpwevzq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2usieesdo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oiiwczmv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2svbvcuey.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gqapcvjy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2otwjzonj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xvjufqqu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mczpqwdn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ezmwmtta.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cilgrcjl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bqmbmkex.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cukxeeia.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ruikmigt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hgxhleso.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kslzzjep.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mrgattvu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2snbiztgu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efkxkppw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpwcsljm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hljtdeij.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnbdxsgo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zyihepte.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgyyoyhf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iprxsiuo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2laxxbtbo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uvleqpzs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkeviiup.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnzxvxyo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kbvkprdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qgdmbsst.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xjcfheue.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ijevzrhu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vsjjcccu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vblofsdq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gsgljbcr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rnblmdle.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2sxgliuab.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fxdjstyj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2daqwtvek.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mpjznott.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fztfaent.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uvprbmpj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kllzlymv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nvmzawdz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2txkmivow.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdvywnu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2knkbilxm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2issrvimn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfjoktyq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yccikyox.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xymkpvez.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xkpfqgip.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2mvlesqis.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxszxveb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2chyrtcys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2mbfppzno.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vezxadhl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kxvlaunh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nqcucjfm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtmxnerl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ekubvwbu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqtrwvgs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chlfnfji.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvdvybic.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibgyoklh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hnsgqxvz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qucjiimh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqdsvila.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdesqqyf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gzadetvw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ubzubhwl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebyasilb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lbijwslv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yznuwlln.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2sjkwyidr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2suihvyff.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2czumzigp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vvhtamnl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gdyzhaxl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2otlfbqtz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2woempluf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vbhphgmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgssrzvd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tdcwxksy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfvtkbtp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2xcvtwxmj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2thkiijvl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wppgljux.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2upjtmmee.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlxyemwr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwaleocx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rnxmltyq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xtvyuexs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2roeiumge.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2eivqaqsl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cmmbcczs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmduhqlj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwhxcuo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pioqrpge.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kguroyfn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bonzzyhm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2owhrdfzi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiysvtxd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ktqwplai.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fpjkkloo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2iorjxulw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ydfrzthm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ihevmkve.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tkygakdc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qvvxteah.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2omqarmxo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xfcqpciw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ungjpzjd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2kstzzdsl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jzwvloxb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oslklsvh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ppdyahqk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pujefchi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzfpkuf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yonjsvqk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vcvgqrlu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2tzwxaygz.html


<!-- 参考信息 -->