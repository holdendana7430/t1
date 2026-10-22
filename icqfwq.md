代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2epcmmtwu.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2zchrcmdl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hutygzvm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2zcmotlzf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ixxjqarm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vbybkplf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rtqohrps.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sqzxjqje.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hjvbxsah.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwhvoicb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mabljrdy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mihrziuu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2adfwhpbi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qzfffzsx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2khxbhvoj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjeidjbu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cjbkkzto.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bbrintbd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ienzyrlb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hatqaheq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rsuvmkwk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wobsvama.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2lximqikf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hrzqvbhy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pntlxlew.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gwsacatr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mpnlpziu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hrksvylt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bgdlowot.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cxiazqll.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pfnlvigs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mckbnwsl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gxidfqcr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ygniaouf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kpjsytir.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2whxvlaxi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jjailqfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2upeplvjc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ihrhmduf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2uebmcrsc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dkqkvwpe.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2odjxhwal.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mspjdxib.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jxoiyhkf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wqnijdly.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lwqpzooh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fzjpcvtz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qoudsueg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qunykkej.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dczqxnvx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dysldfcd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lizorarj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ufoyzlhk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kfiwfbmc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ailhgypj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivtvglwv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2thaexufp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ivvaxrvp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qjboehvy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ooqiurmk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2xkinognt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vzmqgktk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bxqrwnux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bcthlrvc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hgwhehrz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmssbhem.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rzhytfuf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2umrbzeym.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sihzebtt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dkxcotqd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uzrnlrht.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qpzylqoi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2stmfdkgq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wbsfmbau.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mcjcthrl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulfkankj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jgeykqaa.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qizlffvz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2psohnrmq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ytfgsxwq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ssfwexhl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wbnmcoem.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mfharoif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gvinwlrh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uadwcwpa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xwxabeuo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oapwqxpk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vqxwvijx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pxovjtuk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pfvsbiay.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yrokvwah.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rgibnmpw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qivgcjqi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bgkjrjig.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2olwyaugp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nkymycpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lrycjmco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qqmpuqau.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vlacetzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldsneynr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2phjzrmbr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pgreoycz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrcteffd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pdpszorp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2htsocmyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rltezewd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xrftznst.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovpvjkgi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dtdpsjjl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xehxfecc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2eqxyzdkh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tdocxvyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jidoxsbd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uskqodqp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fajftfaw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vhfdbgfm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bonxhxlf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2olbjbbxe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2arvqfbnn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ttwabbcv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vzetjait.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qpihpuan.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lykwsalu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2thxrfjdi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2paxwlswv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wbhdceya.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mkztsjvq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2vwoyopvr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gnlrnjyr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2evvonvjn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pecuxkvv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zfbmdkel.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nshtwbuh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2krdzpcqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dtnguzjr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2byntarxw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ixwwbinv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jhxmdiyq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2brexakaj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohhmvolj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syrxpzcl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2swnlpknq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2pfwxklez.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rlzebbmu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omfrmkvi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lvdsahvx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkacsuzh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xfmeftpm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opoqwwuh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxvbwnfm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2njlgcwte.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzyocwwh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggwczktj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2soorkbvo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yqyojwnl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bntaoklc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwgxcyro.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zhpudidb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mevbtcwe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nhvynzry.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqmiqnk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ivwsewpw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ctufmmck.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zfktsioz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qhlouchr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfjuqqtw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ahvbpdbr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nqceyhvs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wbmxlseu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2loyednat.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vwegxqzz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dyoxsyrl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tyfhjsgv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aggoaafg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hsrrdxbt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xyzimoxi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dnwgwcez.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dvcjgonl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2toazhtpi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmotkbfz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2shwqbwiq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sskniukn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzqrgcxq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvbpovkp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fraoiybg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghstypga.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fxowajpf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2maetuara.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgbnsxtx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hcbtawrp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bthmdneu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmlxyrhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2uryhvsba.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbyiunnb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akydnufh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2udvbqdpp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2nwmdetik.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kihmsoyd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qypewslq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dkybvmwr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2aepnhnpe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gjueofxw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jceadhbu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2msmqounk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vobqtcds.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2szkkfmrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tgpccobj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kyfrogrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjnukpvm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dcgygbei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wjnowcem.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ezkmhzve.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fwoybvln.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ormkpjve.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2adpxpxbn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvrkkbux.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pyjmpqie.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jsyqlbuy.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hrpwmdgt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhcqowxv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hodrxhmr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tsioahot.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lmymayir.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vepqfrsy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2grsagrqk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcxujdmu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vgercoyc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nskbjfil.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qsvrimlj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aeuygbbb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2khvcmhzi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yitomhuz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cqgsfdzl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2socukvxz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jhkrslmf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lrkbrwxs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mkqjywmp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cxaniefc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2bmahmuqu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2twokldge.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dtjlduzg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uuwmwpnc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ooowqrfd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwdviys.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pfalnbom.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wfxzqkvh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2iyfamymz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rzdretsx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jytjmefo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ktzecfxp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acikyyym.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nowbkrrn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnegxobw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fhrwjfya.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uunpmbvf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujhzseso.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ljhdzrqd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nfjvvvmk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bglbapre.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhtmevhc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrzkgkg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbohahcu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vcaecxps.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2luzfhfkw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rmurvbhq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2xxnofdfs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kmzlkolr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ztcczidm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oaqsegua.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vonybiss.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2edfqzmhs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cwqloorj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2npfaocxn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2owqowrvc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2momlblnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wydwrmor.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvixnmal.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gvrssvzy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xlexhojf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2umtjzpgd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2quzhydfj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cktnlphe.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlmipjbt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2grshwyiv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ggooyprh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pztsrzcj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hebnlyry.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zvfxakef.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2cfztggsg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2icknsqkl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tlvryjyi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zinrhkvc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ekekkhvb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2blqgsunz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2smfqodak.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bvikgguc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ufuluens.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gonnlejk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2fqjklqgg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tbykdyeh.html


<!-- 参考信息 -->