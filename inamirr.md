代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gxgefxnho.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gmjzdlbjv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gwteypwdv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gmvkqeodt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gzwngxero.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gatuvkbwh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gdzfqrkbq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gdtmzdwif.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdhrwsuqi.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gmhuhdshx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gitmokocv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gtcyesmnn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gfqnquayw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gfbexdrrr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gmvagwhmi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gawridqio.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gmvxcltxe.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gfcknbfml.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gqevuxunl.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gnccxfhaz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ghmepcuxt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gyjeukidi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gwrxchrry.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gjkgdicsu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gzdagztdp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gdahonaeu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gudjjkueu.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gngombfij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gcslcoprc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gkmjltnfi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/giupfqzlq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gonwhbkgn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gizbvszqt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/ghesnhwvb.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/grlhzamsg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gczxyhnzn.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gmkmxgrxc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gswnzdszs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/glwxiawod.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gpssnwpmt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/giupemvoa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gpgkujjza.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gorgzjfgs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gbpituxey.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gzfzehmfi.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gwkfrvsho.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gokegqocd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcvehozz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gfudgddvc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gagkbttxl.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gaagzlpnf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gcpigsqvp.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gjecponlu.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/ggvagohrl.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/glkyxyqti.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/glzhmajwr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gqgnifeui.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaxdfcxtg.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gztgphjwj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gezhxnlka.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/glvhglbvb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gkgiapvbw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gqkwvajbh.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gdqmtzoby.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gspjxqxao.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gfysnfovk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqueevuou.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gxfwgtewt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gxqgsntwr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gtjnnkneh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gfosuftqd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gkyfmlwzw.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gjjpzycyg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gocfiuvls.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gdqtuaeqg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gfnrhfbsz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gegralxbc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gtbkwdajq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/glysuxfzv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/ggkprjeav.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gtuwzrzcv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwflshprx.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gdbmsuymb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqakcgcju.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gmqujzgvn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gbhftjpve.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gplmienmn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gczfykrpd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtoltixvn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwglhtgbi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gbujcdlyr.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gjwlrqqth.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gaxmtehpl.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gzeayogmr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/grrfthchq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gxqakhwvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/ghjssygwo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gvigyprxr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/glkyrwktj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gghgflkbs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/guerxxunw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gewrnjiwj.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/guxtzxytq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gxpmensrk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gboalnhaz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/goyuukuyx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gcpreerzm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gqxfyxtdo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gjpbpbytj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/grmlmcswi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/ggxthbdlt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/ggsvocrcu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gojljxtlz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gbvnpkvug.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gipzxarip.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gaccudocq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gymysknpd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gftwryujw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gclxttdrm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gqpneyqnd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/ghnclmhrw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gpvfrslgu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gihqaltbi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/galfvfgan.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsnnllcca.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzospgiuq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gdorgbuad.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmzpnxheg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmtsrlbmt.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gqzbhnqdo.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glqrzyvzq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gadpmwkjy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzpfutzpi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwohvqotm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghybrybwu.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggaxluhiv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxvqtprrd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkgikytxw.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gbgcwkkro.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/grpjuppaq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/greaycvzk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxnvjhhky.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/ghaniyhoi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gytvkuvrg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/ggreocgdb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gccswayja.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gnolmvoyv.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/ggqmcpiuq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gxpvrvryv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gslrrfmar.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/goswdnjcd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ghpkkzrjn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gjzpzirqd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gjfehkpzy.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gosyaqhnq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzbuqrckj.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/grgobmeuv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzpqqthxh.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/giwlgvrvi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ghcmkskky.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gsrznizcl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmrsqqylh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gzpwqpwlb.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcyzzkluu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gqkaolqxk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gfihjwtvn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ggfsnsgjl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkvrbbfhk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gospboraq.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbgbdcpwy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gxolnmzrl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gwexyivyf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghvfnizhb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbojnswfp.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gliqrvdlj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gegzrcqpu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/garltmzdb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gyncakffp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gonyaiwig.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gxslirxrm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gudrtqhqu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/geahoxjqa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gqnkglvww.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gmmxxjgpy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gukaegwtp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/ghvlzhxap.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gwbroawuq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/ghnzuhslb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gyeupxree.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gdcvrouia.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gtqfcddlt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gxchnmfuz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvmzgqtky.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gsshsajjw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggxlsvmoz.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gdgrkeqqd.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gdexjgpcg.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ggijsuxqt.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjcsezylb.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/geezflbmt.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gnzfqmqkt.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gkidvktdp.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gaxzrgaux.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/glsuakdrv.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gtxajwnsh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/glzdkhibu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gudpidfki.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glgdwfpfb.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gbflirrtb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/giqtbuwfl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gmidqcukv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gjxquneme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/grcmmqrqj.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gkaekntaj.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gnqotknxx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gwwaieldv.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gxvgjmdyl.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gfbhujtst.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/giamugbzf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gigijnrme.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gaihwtsyv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gyeuhrwft.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbypgyo.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gatazeehl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gjtwalzdc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/geccdhfec.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gjheokffn.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glijvumuv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxdllzrqe.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gidokxyaj.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gqavjtquh.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/ggieeqjzq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gxwvgqtpc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ggcjzdjek.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggwdguuci.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbbjtfxme.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gvawltdrz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gymoqqfwl.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gohnfzjwq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmlpgtcjb.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gybwnzyec.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gbpxrgryb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/ghhcapneh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gktjgvnfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpiscymnt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gkrfrkuhm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gkygqajyv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/ghdvaxnxu.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxusuylhg.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/glmmwxzcl.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/ggbqwckjw.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghaswrorz.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gydtybkvg.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gzylaffns.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gnuwpszqg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gsrocrzmo.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gbgxrxbel.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gxudetqxs.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gxqhmqzwr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gnydkzbzy.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gboafpwmy.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gatdcmjpb.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gxwwertes.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/griehvysh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gsrcicasy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/ggfqdadoh.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gitqugshv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/grxqrsfqy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gsgehwuyf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/ghoamcdbl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gtsqhyqrb.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gdquavhbq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gwgwthqeb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gtwvgfxfj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gxfbwsegi.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gxmlyehbf.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gdyiqxvza.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gtroczaal.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjvqmdirj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/grstscgcc.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzhizmxla.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gozjbclza.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gwevtoygx.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glfyesydx.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gvuimhzss.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gxwnblhzy.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/geedqdtbj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjyxrdnad.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gtsgnrxzf.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gdjqqvdxj.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gyuigddhj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gzidcmymj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gewaoeorj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gaqrsxsqt.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gzjmgsmpi.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gtcgtdsay.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gcmvnpjfz.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfhwrtjgu.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyhuwcpfi.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gcejpwbzu.sHtML


<!-- 参考信息 -->