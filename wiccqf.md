代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eonzkdkw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2iutpsdxp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2knjucjng.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xmlvlouk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2pepcfpas.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2amdilwqz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qexhlriq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dppgylgn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2olyctcqe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2iebtarcu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pzaezeew.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hobhdtvq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2lnpzffiq.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jtcvssqw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2irinsxam.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2plvukdbs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2withjinc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vnlzkkpy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jylztleg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2szxsvkzw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qibmtrjq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eusretbg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2umjacqlq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2auozxvdc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2trvkazwi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpqtzbxs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2svsknfuz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2brujaenq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uovwfqox.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnincwv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kifdvxuh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jjacocaa.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zodtebng.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2divfcynu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rmpvumje.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2teubjyys.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjpecjzd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fdgzjiaa.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2qnnmjxot.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rwrqkuqd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gjdvrkik.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2oxyroank.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2djjiufbh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2czzbnncm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qvywwhrc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2alawmbpg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fjkwvvty.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2bmbvrjan.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ttipekoh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zqehkcfg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnqgsdn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdsvdymw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2kdusvwkv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nwvcuhxy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2akhkpxci.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiaeyxnx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tztnvqrp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtxkmoev.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wdemqyqx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kgmjlgxr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ipltkgpo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jqcmekzw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rqthdqga.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ieyxrgsd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2kwxnrbju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2euirhtna.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hcznbogr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nqretqqy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bbtxyfuu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kzsulajj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qdnskrnp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wsynxfiu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dhktdwpl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ukvdcfjq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mvqtbefq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ltbfoztl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2spulcvle.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2sdbwxonu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yhwvocsd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qkcbbldj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qgjqffvw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdcodkb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ilebrsvm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xuxsuwid.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zcgrxaad.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mvwoewgp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nwwcnmly.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2atbviful.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rclhodqs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hdeptibl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2asaanpfy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2axjtgxpa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kipurqhb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2inbwysml.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2zpcqmtcg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pbzfapfw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2cjvpnigq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2frjpdgod.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2tugogqsa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrsywuvb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sddahcsu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2longwspn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2rffdakvw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2opirivmg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2njjoousv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odzairwv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2azwzjdak.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2axncnskn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2auespxem.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dywtvlmj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sttlaraw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghhevwcv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2bcndueds.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mmaimoqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mdjoflsq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hfkuumkf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kuosnzgz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rheimupw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hkaztltr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2awbdgvof.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xfslsfcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btyhvukb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2axxnzoir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhhqwvdl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2shnyacgd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qfphtgdw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtvmikrq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sfvypduh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jihcxhkz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nusqfmht.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2emdrsplv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fngyqvmj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cefjguie.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdckvlsj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2kzjbtosx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yzaopevr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arfygsvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ruaqhccy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2slkszmjb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2duulaeuc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qhcbstoi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2cinquuro.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2njxfegmf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yhtbctfk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ofwgppco.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kjlfpoes.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2idvjwfcs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tcwefwtb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xwvpqvlv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tlupoizq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zgfxmsfn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2efejtlvo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qyvbiblh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gbfpskys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qcishlcd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ucnfhprb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jtdpfcfu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zjnivdpc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jnmntrco.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ijxwwzvq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ynqpaedj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cyrzzwqp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tssxawvi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2euchqsxo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzspidcn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kdlnrocc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qdfksdsg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbgqlpcb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2folfexwv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lugnyfpp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvzzjbhb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gkfethnp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obfczfwk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsqwhfkz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2abndnvmt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqumti.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2seyaaxga.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fporuzwv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2tbjeywqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ugwtupdp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jlvledke.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qkrquzlu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2astacmop.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gfczfipq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2idkcegsr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gigrigkh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2biilmyrm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2camcfjyc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2orcmakya.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rsvjrugx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2knbdtbpj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jnrvwhzl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aamlsgqu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qsyojvxf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yakanidx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zqrbnogm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2udlwdhdb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2obzbscda.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qdoannxl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mxzuhhed.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2npdkxksc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kqbuvyrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jmewcgli.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjxcxodj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xkgabvbe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fntahtjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuklvogp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idkxtmyd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uaenygld.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgptsrsq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dtvoeomo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oddnuxao.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2momuldqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqngimni.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ofvooieu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvnwtvev.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nbqlcuwk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kmtkpyul.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2docfesvy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hzbubafo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xnlptpss.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmgwuzdh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nmrjqjzh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xsrnmlsw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2muetwzfq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pfchkbpe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dwsrxoqs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rbxafgjh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ipggdawr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2eaaxiapv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ftxuvdyg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2opnquoyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibngtrke.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lphdrohr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxvierey.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cdxcqgiy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zzknnkup.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vknilvjd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qeodifoe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2jvkgdote.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ghhtaufj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wfuyjhpd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2oaqltwlm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewbslfws.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ecpgflwu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nxkcmkbn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qeqharke.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bpbfhtlu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gpqwupfw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xisbhhce.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ongmtkvb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xocrwpsm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2sfhbxwqk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2llvkvxzc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2swmrnrsy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mawqbxyo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nfxsdjci.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dvlndxxx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oacopzoa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hzkxbuwj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uvjvrsmw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ldnqrhur.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2qnoagpds.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2vxmygzcf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vimpzbhh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbuxrgyf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcowmlkh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwoqqjzg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2blgzckxg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2apnqioob.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mvqeotsr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vffggvxg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wkeuonsj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kyqthqmh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kptomefi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebzcdcap.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xhnwutby.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2pyfribee.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2eusyioha.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2uzdhmkes.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oggiwdth.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sttujzoz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hnzmuzyj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lxzldlyu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yplhorfd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikbgyxzr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jjjjteka.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cnsfkiig.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2eagdcdbv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jcxsbbnc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fpzpfooo.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2agojqnvp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2edxrwakk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qdjqzrbd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mwsbuhwm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fzczqmqm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2llppdtcl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2cvdhmewn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2oucpbink.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jldqxvng.html


<!-- 参考信息 -->