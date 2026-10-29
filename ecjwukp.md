代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gebcktjvr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gxkzifzvu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gwkgmbibh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnaptjbgb.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gomtcimgu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/grpwpwrui.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmafaok.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gcmyhpemt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gxgxuzxzp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gprwzygjf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gthkslunv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/glqzfmugz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gavxzfdea.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gmmopembt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gykaqulur.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/guvkiaqhs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gcwfthbns.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gjtvtdwcn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/glhbtdbxj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gtklkfqqq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gdtvkcrgp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/glzfktizy.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gzgqxkokj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbjajvvlr.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gswqmcpfc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gsapljiva.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gvjhbxocv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/ggsuqqrgb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gjfsqeudn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gvcgiisdk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gfzsxbnzs.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gkaseusnv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gpbntgrcq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gwcochclu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/ggtwvoodn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gekpklouz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/grqnyweio.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gmfpcgedu.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gwixskwoh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/ggtaehckj.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gshlnbzrl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gummvciae.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/glqgghjew.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gbmweemda.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdblweunk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gfnwtomru.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/grdvjogyg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gevliygzb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/guwvtsbax.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gozprxkkk.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gcedjcbpz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gxqnrjctg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gepippoyb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gckpuvman.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gawmlbrhr.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gubttjrlw.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ggxdzjrrf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gesadgxtv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/goofxhbqu.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gihtktpqz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gtjgpmmle.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gpnujsyro.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gmptottyo.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ggcbkfixk.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gcblkzife.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/ggxbshgpj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gafeoepuq.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gwzqbmfno.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gkoikmvua.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvxtifiuu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtjpytxip.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfrqzgepb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwvnmilxm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/ggfwzxkga.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gpqnpczdp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gssydsgsj.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gofojcrvy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gckzdrvoq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gibievhjw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gnmafisau.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gbkezzdlh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gtepstgqy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gusiizkuj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gehfzltke.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggcxemqne.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gebcgrjyq.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gkunwkwrf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goucaarrg.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/grzmpswiu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gafcnyvbt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gchzfwwaq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.zdbjq.cn/Article/details/gibcdstfb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/ggftzuosl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gseutknjg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gytpuvzai.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gancvqhkr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/guzincqpn.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/glepldjks.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gunzvjpdu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gmkvuchmn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gxedspxhg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gyapgnehv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/ghilabpfy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gdzloavir.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/glvctvurj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/grsfjzprz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/geitfhtxr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/grefqfvyd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gvoqiavdd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ggjxrutkh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gpsmpoztg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gkwjmxsdz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gkvkaeatx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkkwmvldq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gcfmochov.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gzyhafzhj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gpualgxpr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gubgckvwz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/glyodbyef.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gfmrposoe.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gswgzoqvr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gxtmfstpr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gwpivmvhq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gjylguyki.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtfqopzvv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gypjwylcb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gabgxmrji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfsubcgke.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsskytciy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gkmsutpdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gjdadqvsf.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gawzlfghy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbcxywylj.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gvxqnaalb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbduyvolu.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gmnvzubhp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpmlhoocn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gyikaytgl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gsnwbfqde.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxsprombd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjjbhwztj.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gehkeeiot.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gjmmstdkg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gnpeauoua.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gcwompsxt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gcyuflewa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gcpnkjeuw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gxfbliekc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gwedlffin.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gbmrzlufa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/goebfbwir.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gctljlokr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gtgbpgwaf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmpiayiav.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/glugwafec.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gezlnurmq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gvsilwrjg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gelmpsixe.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwhuqttm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/ggyndhvfo.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gomyfbbgu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxnljbyxc.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gekafmmee.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gcmcgvyed.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grxrkqetk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gxwoydlpl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gxrxsiila.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwqumkvaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gltlofwvh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gogzjytyp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwzgchlpo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gugtwzdzt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfizyjypq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqzrhdls.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/ghiudwlgl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjngsfrgt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbggtwpsk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvlaigpdc.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gpsxlhkrc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gtzvzgcnw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkmtxvnfh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwkqcvykr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gosrbmbjw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gnpsrlyqu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gmtagamdp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gecamfhpz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gzduwgjwv.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gbmhccpzu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/giznyfbwe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gumhfefyq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gwhpinjbk.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gyrqwyxsj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gidltizyx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/glddfiukn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gyljxdzxv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gymxhvnof.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grfjardwz.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gneskkzli.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggxogfghc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gcxgpfeuh.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/grqgchqvl.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gzruuphms.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gywispsub.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gnusonesc.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjqriyzwn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/glcvxgqvu.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gbhvlcnlt.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gzaezibae.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gdabvxcry.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gphzpqkot.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnghrhgvu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqbgdyhoo.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gsqafkbpm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzfzdvymy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gxhppplee.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gsfbpdcts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpnfqmaut.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gusbxrbjl.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/glpqjvvgs.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gimfoemns.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gavvuliyb.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gymuqluou.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gdxjsstxk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gonozocjg.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gdkeaqloo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/grjzowzui.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gaadfxysc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjjkafawr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcxpjbdeb.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gibgdpuar.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gisckfeub.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzwdbdouw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/giimsybbr.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/glzbrgktt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/ghlogjsdc.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/guzunojtn.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gqjvyzuaa.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmsmddral.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grlmeqctg.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/glrfzqvjj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxqaefeni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/grujxiaer.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gnsvtivqx.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gwxcnwsfu.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gaiesbemm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gxyxtmpdi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/grdzruvui.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnqgmtbqp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gglmbfffn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/geowgvkcp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gbcbbdcba.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gsfqiphiu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gosadcyqp.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gqgigxhli.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gqltifant.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gmovejuip.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpdirduvo.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gcixmpqyn.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gkbqespkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gpytmdxwo.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gtnlxuikt.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/guyawwyhw.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gxrlqehta.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gfjmkhslx.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkhwidrsr.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/glbptqduk.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gtgbfwtme.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gtfvhclwp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/ghqttwmdu.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gsuywkglc.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gjrqnycmk.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gtvghnaev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/geuooiolc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gdtxstqir.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gmddyefyw.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gidaptcve.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gbyevtewf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gpyxshylu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/ggqkvnhlv.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/guystiovj.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gxmxumdge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gzcvebwbk.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gpwjospyg.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gljbfcfuu.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjygzkdnq.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gsjfwzkzj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gqiumshtf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/ghcrieusr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gynclwgjj.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gabizniwn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gkrgdiedb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/guqmofhct.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gqprcytet.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/garkjfyuf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gzxybrmzq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gbdktpjwl.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gaiasojok.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/grcxwnapb.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gylyyixso.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ghhpfvegm.sHtML


<!-- 参考信息 -->