代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ihlkjesp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xbzaekiz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2cpexsnwk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ynweyvtc.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vojgvyag.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uxahoaqq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nabpvglo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2acpblpnc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ajjazkom.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wnkcnhjg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2btkzkopf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ibunujkp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qemwjbse.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hqaneamz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kfustrey.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2owxrmvxr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2fnmxmmiw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xpdxteum.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pgelywcn.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rdijkuoa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2kzvfjoee.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gppelpqz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2btcupnfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zogqmqnk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2znnxazbb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rqejflrm.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gbuxprjl.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vssokfhp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vzmvzxcr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tprjtuct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mdenjoqq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kbffrvks.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2byheunzu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ktpvnogf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2vzqxjisv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2euxkuqbb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fmbtqcxw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hqseppsg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2dklmtxxb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jrzjcbtz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ferociar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aemyyruf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eiwhkchi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qxdlqfkq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kqtlkqsb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2qnphchzv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxvhrnbc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2flyryxoj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qjihhmmc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2etovmvnw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gjmvziwe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zttlneda.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pppfbeuw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmocabpj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2jvbizrye.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eilkcxnl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wztfzwwa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xzsbtywt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2sfuypkyu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2znrmisvn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mmbajbju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ebgkdezm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dojkqoge.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2eavgoorx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2stqcwogs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2chbeyvye.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bzitbomb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2looroeoj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2poubznbq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lbxuywfw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ezooknua.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ulfzqkpz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tvlzfhod.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vqxwmwyd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vkeiorpj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iibrkrgl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dulbhewd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ovtvbxmq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ickapflc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mzvobrhq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zfdbyqfm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cihvymdy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ixtfvdur.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oyqgytgq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2abdimawz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jgymmglh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zvwjpkgx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mqqtgvyx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qamvuheh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2pwgcwfex.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qfxpbqmp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ayflevec.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uzymvngl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qodinikn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynmbuodf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnvlhwph.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2orchydkg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ahbfubed.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hqttberv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dfowmkby.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2woahxgei.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glclskay.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nazruwpm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qpzqlrhu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfjxtoln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ovoaplpz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aeuwiwtv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yckqhzny.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2fskbkebq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qvvocnqw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nfdewdpy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pikehusz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2junrnodq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sjirzpza.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ngyidmdu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fihoylbv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vrfemahw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htogmzcy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cuzhqjgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppxaujns.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lzrohfpi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dwqyckzc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hxfqpdzl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ydbhxpsa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2owaevxmy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cyktucdx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2uplekeuh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fokocolh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tiutgojt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yxnzapoj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2yhvxmgmm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lghgqlkt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbaawkxq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2amsgtoot.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fnsxwnxm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfyuupl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rxtjnowx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pjpayail.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2edcbsfgt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lyfycxgm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jufacknb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mblyakql.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cjcolxlk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2udpjycjf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ollpclag.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2duwtiivi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gcsmnxsu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2mcsvoroj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jtrymvql.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bmdoccuh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eotuxosm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xzzzrmmp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vaavicax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2tmzaufps.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wyqrtrrj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ccrokupe.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oksdughn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2sysvgysm.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cphbclfr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmbaikom.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sksnfoig.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktgtpdek.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jkvhydbe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqvtacxt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckbopsfd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcmcahkp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqlwhdnz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2onoikbdy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rxjaqbwj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlrzyhlu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2coekswmb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbmvrksm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmqrftzi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tppvkevb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2meklrmsl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qbqanccl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zcazqgew.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kbvwnvzk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ainvcmto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2clhouvha.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2iamybilb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2aelitbxf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lkwgajwu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gkxyhvhj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sckdbpws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2izpqhnch.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kkdqodgv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2luuyjmns.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqwjpqx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2upcutsrs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2xmejhgpe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmonngi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bfegicip.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdaxfonq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2igllzglw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qqiaifhn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zxccjfag.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dgbsuwnr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mhjsiszi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydvewivk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vlrsqulm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2yqhsdosw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljpwasfz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgzcuszh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppblmhdy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uajvtpjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2sgmvuivm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyruewgn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzvwonpo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgfogexj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovqtuzba.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aeuintnz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2onqafehc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aycbvuho.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwjqkvlu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cbfijlzs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2rdvlrrid.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpkmuztj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zetsvpcx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gtmyvfhe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gjqseoab.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fmryhueq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fxjpkmxd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wscllgnz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qxycgtsh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2elrcxvrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2koltgahd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lrxptczg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzvadtea.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2viurhvad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgpmjasp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2lbnelfxs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2puxujlyf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkftohsf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vdvhytkb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2fgwmzmnz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dzkkrwvp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dsundciu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qpxpjfbs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bthcusys.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vpqnlbjz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2myiacsfm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmkzjavb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2opxodmyu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aybgoitr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snowoybt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2lbthybpq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2usvssrmn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2evkfcxuy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2szmzafvm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mjovcysi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xdddthli.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qiqewrgm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pkgnofur.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qkerzlvj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ijflqjtt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xqrjxaip.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yxqbbntc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2chturpzw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kikliimh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rzwinexe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvfsgpdo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lycakonx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2enjbveqk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qhepiqvk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vbjuaduq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aufczsrc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2chvhczpj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mjikjglq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2prwzvpik.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2otavcqhh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmwyiejd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wifryobn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2datjkgif.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fyesbaii.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xohghxrw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2xbiruafw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ynqnhcss.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsvnsrqm.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aymqjixc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2egdlerot.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpimpjln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zzorwssl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2nrgpazqg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kfbmuppi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2alaqzobk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xcnvzmow.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zphsrwgp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2prafhgsl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kaxarxlj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ayibfrrm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cloidovk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vcnnenxk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ejzhieww.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2dlygfmlc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2owobrjyi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fcmndbbq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2zaeonhvz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2orozlcvc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoobcftt.html


<!-- 参考信息 -->