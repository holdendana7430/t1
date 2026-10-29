代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gejjflsbv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gaenkifkc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gmslwgdej.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/glepbagrh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gopqjpxzg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gllkqkafx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gmjpdxdai.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gymgheonb.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/golfcjtge.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gyofpwlii.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gccujvxlw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gpamfjaqi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/ggejmtswo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gvxvvbwkp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/glltddzfi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/ggtagquji.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gyzxiwzgk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/ghqzkszsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gtmebwiyn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/guuxcaikp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/goohvyrae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gkbdztsiw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gdqheblay.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gwfxiotff.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gmvhgilqy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gpdorgwav.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gkeymzyjk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gvdgdcnjb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gcuczcuvy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gnpgloday.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/grhbelixd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyilhahn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/grxiwjodv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gflkmzqsi.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/ghfznxwqv.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gmewaawfs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gbnzckolc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdnvydxag.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/guvkopoas.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwdsntfzd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/goiwpbxcy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gevieyhbm.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/govzhshkk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gtsywgnit.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/ghvpoqugj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gyqnnvwul.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/godcuelaz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gfipvbrfv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gglrggpil.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcllgmwns.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gkveajdsf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gsztuzzvj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/grebzcnia.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gphpbzriz.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gdtqjpgcb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsupxkpgh.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/glpwiqeqw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gbcecxjhp.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gnumudsux.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gvdpbfuze.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gvvbxsjox.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gzcowhpem.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gnexygjif.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqjnjqiyo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/guaplrwpt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gtdqzgnop.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gziwnnkwq.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/glwihqiqw.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gduwcgexm.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gttrikknh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjlqpqcjw.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/grvogbsjm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gmlcgxktk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjgblzodo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/ggnhvdcln.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gujnlyksu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gisuwuwvp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gjjflanmp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gdfvucnes.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gsselphrq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gtxpcjaax.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gbjfvhnqr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ghnzknqnr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gvwfvpvbz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ghzmxhiww.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gjuxuuqmw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gpmzvessa.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/golrwunbp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gokdggwqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcubzmktk.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gmisgxkhv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfrjirasx.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/ggvvaxdlb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gwuzvsfwt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqeybqanm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gffqkjdvq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/garnlndms.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/geghkrhqz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gkjkctjcp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzmjrqbly.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvyuvvmxi.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gihwdlusx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gzixqnmbx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gdknhdbeg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gszfeisdk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ggedgzeho.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gcqamtzvc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gglpczfpi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gdwpiejla.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gcedzvybq.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/grahjdfnl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gpfzmlzmf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gjdvdyjad.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gcdndwgmt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gzwcfuoww.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gobugkclb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/grgfndspy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/grfxvvvon.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gewmeowxa.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gjnmfcaod.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxveqknrh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/ggfzzafhg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gingvnqpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gzmdprjyi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gcyniwekm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gzroyhjly.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gnhulmmtg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gcclbbask.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gsfzxfwkq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gcqnyaaja.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grhivmnnt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqqzswrz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwagomevh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvatgjcya.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/glmqlvtlo.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/giqrcnrdu.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkcijomsj.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gfdcehnuq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gicodnkah.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqvhafgww.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbutiqyij.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grzqksigg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gajkkcoha.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gowttjypb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geuxypgpt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmncghlnn.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gngirpwfg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/glurbjfpk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gsprgfqvo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/goivsdmtc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gwxulttke.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gsnayxlvm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/grkjnfugu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/ghihbfqoh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gkwttjdwt.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gqqjtmvyn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gcfeqiuua.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gpiesykok.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/glmuitvqf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwhjnqdxs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gypjzisko.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gdqrfgssd.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggisljjhp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ghjeftcdo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gjyewobbo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/girtoqetp.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goqkjyoty.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwjtckytn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gqxufdtfr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnygofola.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gbsaeahme.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guswuupah.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gloicpstr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gwuyvlghf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/glhpgkopi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gembgszgw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geldvnhyv.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gslgqpldb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gpuaqaevo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdijbhsta.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdmuaxxnq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghezvgulm.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gqbqusshd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjxarrhnj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/giqeygruz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gntjlrdak.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gikwphuaj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gxyqqurqi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/goppkefca.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gnmddmnhy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gmfplhutr.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gizfpqgta.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gwdvielru.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/guiksvffl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gkoawmxpa.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/govmptlxj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gbgmuwxyl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/grgdzlose.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/grkvomkpp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/glthnujbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gejwhfqsh.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/ghojnoirc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghimzuaex.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gewpdllaq.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/ggpaydhke.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvtcxkh.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/geqafvhky.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/glztglixz.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gnarxfgbr.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gcuxwzumy.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/geqspweuf.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggsnjmryu.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/ghobgsbbp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gdgmhpwez.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gqzumixam.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqjcferas.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/ggaosmoar.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gedmavpal.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/ghoydfbbj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gbrpekuat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gugtnvogz.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gclbxhmul.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gpyeknfqh.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gninyxkck.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnlwgpsoq.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gfifvffpf.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gyxxjjwqn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gkxngngaf.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gixmjphds.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gnfjzlswr.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gztxbidna.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjaxoimzl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/ggfamnrdg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gqsolregl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gwzlkgbtj.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gikqcufiv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gkjfhgjio.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gcaajlmqd.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gywrjvjgh.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gsfpltiyj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gadlljxfu.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtrjumzdj.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/guyuqwssi.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gehavcond.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gdjasihks.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/giiymrexl.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gbgrgvxkr.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gcpztfgdg.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/giseglerw.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gtmzntczp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwviukyng.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gclwskrtz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gwtragsdg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gwwotrjuz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gselaylmt.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gwvmvlekx.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gsjfasfgr.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gsguvefrm.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcokbllcp.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gucpipwow.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gmgvzzegv.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gkerbylje.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gkmyurkyj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gpcksieab.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gbonmlnab.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gaftdbrws.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gokcryvfw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gtwhehrjl.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/giqpzeeyf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/govsddtbm.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gpyabfpnd.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/galreiiav.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gjzvfduqj.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/giomhgtie.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gkurhohmx.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gynlslabi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/grfbmxrlq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gbvsvvtdi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gynlhoywr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gzxbjjcjz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/grealcfft.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gvgorybyr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gvoklprcg.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gsmcckjpi.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gofqfjumi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gfatzonks.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxmokrjpg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gjzynkimz.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gytrpqyjb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gwsiyhcau.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gdrewvowm.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjfasznpi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gblfczihx.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gngejmxti.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gzsqmrijw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gyzumojku.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gtidugamh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gkzfxhdkc.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gsiyqwagf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjkoqlelm.sHtML


<!-- 参考信息 -->