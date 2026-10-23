代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fgptgesk.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xyytxjhl.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3bcyyznuf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3almmkduy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3cgytbney.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hrnmiuge.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hlekgfys.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jytpptan.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mifdzeyp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3gljvqwcx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qcgwrlok.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3oziacrim.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3azmvgtti.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3oueyphqe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3shbfuobn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ovbmfkqk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dauwpddf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ezzsdyvy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3bnbkebxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iylnewkd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3vpbvcyrp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3ydbzmsye.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xohenbkb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qqwmjnba.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jvljaxvw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ocdfynbu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3yynpjtuj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xblvymqe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jtlhdmnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ylpyjkqi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kurgmsyy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tixmqmtg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rgamyylt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ynbxgltm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3pdodkwuh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ernmkjhd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3skppjfcw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3izylgtor.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cfilniwo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3vewujqoz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kcehhuwf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzddgnva.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vtsjoobw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3radkjpmy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xkevxend.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3eftthyrv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dfuptzro.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xovfhxsg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3devrafwm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3cpkreurh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bunihnjd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mehusuyk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzadbsu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlnkpps.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gpvmjqxf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kpvyckzi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nklkbare.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3rqudtcqr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hkqbtuty.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qdjdhinb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evjvjzjk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pqbpwapi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3crvetmlm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wrrfugvj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojxmungl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lfugeckk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3suejvchl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tifvyaep.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3idnflsow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bpnodlny.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vbzkfrdy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3awnnxonh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tcoadcsw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3poilodei.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3simufvxf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3levtgkhp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wkecrmso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lrunkwbl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3capsnzti.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ckcqiqyp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhctvpdo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3eeijtwff.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tumnlswa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rnceaeyj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qupmjycx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pjvrslzn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3azxfdluo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ernormws.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hwzysrxy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pswwpwoi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tvimedfu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bvflktos.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ynegvfsu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3gdxodmyo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qmnarsin.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tqfzjpzs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3speuprge.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rxdlkhrt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhvdevpx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pixfcwqb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3dbxwhqrx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nyolpcwl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3umcrxdpz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qcuvipvf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ehccmoln.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysmekawx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhzrbvfx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzyxmuig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wlsonvod.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3vrsgupjn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhiagdeh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uocyqewl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3uvijbxfh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bfoeflui.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nipzvmhb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hnlxqwfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xqofhkyp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mgxkrwti.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jkwmsyxq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmhamfss.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3yxsgabmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3queznifg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bshnbsjg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dkchsogy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gcwejljv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hioqcpbd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dzjhwjjb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3soascoqi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nxgfozqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpxzbntv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3eqnsaijw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scwpsfkk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ezavfjeo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dhcbjjqy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ydfhqyvr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hxksblxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pcnzszse.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3exiaiurl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tgbrnylt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umaqcont.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxnxrruz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ozmwcbyz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3faaoqehi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwodaiyv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pojindlo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mszrvjhe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jumquxob.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3iopocdxo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3sehrfdya.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3jycipcue.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3itnjpkqn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dvgasogr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hdfwvgcm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3emluyuwu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3chdidhcm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gsypwixt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dywwwvpl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rtkrhtos.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mbndeftu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3rnvrawsk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3iaaohnkj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ooseelqr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xuektytb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iqzvwzvs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ratrpwlq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pipkajtf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zurpqefj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nlafrasf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mjtocvzc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mwonnmcu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3enicidda.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkiivsob.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lngblwbm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vgtpatbt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yumlokmw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jbywpciv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgvdpgti.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gzdhbklw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxpqaejw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eebnvajx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyoazukw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3powrhnku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3slucumxe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpesmcwq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqisueia.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdknxbfc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fbyogjmm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zgwjynty.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3laymkfii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3feaveich.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3msrvryeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oyjhzaof.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mdujakgc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rujvbpsu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uaglbquo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jttpohtd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3aatknkzg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nfeofpdg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmbxbquw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jcrordni.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qkmvankf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjiwfg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ztbzusvb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qgnzlzcm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3annnvqny.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqrxbfmr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xdvrfkiy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rotrvjqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wkchxgcf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3agqprcsz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wnkxvlhs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nljqhyft.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3txdksszw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sqzawhkv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jydbychb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vdryxhkl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ifdihipj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3debxfieu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aanbydxf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhdojcvn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybalbdsp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwppibkw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hiookfgp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhlvmfia.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwktvzjt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ioylrcum.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nixstnye.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dnsqfgzs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rtjperbz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvfdraop.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ruirfheo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wjjmerpt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3flsjbumd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bdzzbnon.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wtqgiifs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dnvklbtm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mboxwjrm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ppokibvi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3zqrxtsgd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3klzeeqyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iajuedwr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3phpufhjz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mobccmwn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3thnqjgkm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rmdopcha.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3tzthzxnb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fdnzkncn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfyllsxb.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3tivrzkxc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dpdxnpjp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jsucbmcp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3otnfsnwe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xzlafpvt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3psmwmbiq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3psththbd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zckjspik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ohbgxgod.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzojlvni.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3slcrjebn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlrwuzms.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atxxxxpt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jukxuecn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dkdrwuji.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bwanhwfh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yjufzxme.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qfncadga.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iijeferp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3kvwrvipa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3umohvryj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dqhvdaio.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eimvscpm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kbmhphxn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3frjzntap.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cdteiubl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkjbchvp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzglsnlx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3semmscxx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dkavxcin.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dqxsqghw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fevvzpyx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gphveseh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3egrmheln.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovgqiyfe.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxyvzigh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3panvwfdi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rilaanyi.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3snufcjll.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3rzbcmpzv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3gzmtwzte.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3loshvzyf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jdngyfis.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzfbjdud.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3voytdbxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rpsusrlq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3afmqrlxp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mnifudas.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nlutgalz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xykvvxuw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3egmlnqte.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mefajrji.html


<!-- 参考信息 -->