代发 wailian999

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gykkbdvsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/grqilqumr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gatretqkg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gqvfxtdex.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gsgsmjoyt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gpblxcamu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gmsxmehbt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gaeavaoih.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gjwaerowi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gewrefrzy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gwjeuqmto.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/ggmdbxrwp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gwzzlbgcw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gznuhdyaa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gjkdcsmzr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gltsknjbo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gbgoyzcqh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gorcwqajq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/glmndqzpu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gmvotapbk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gboiduinh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gjibpamrp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gheyjbbgq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gpfzvhjbq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gaztgyjbb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gocespjmn.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gejjnxevl.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gabnvviah.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gitjymnlt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gmgtiikzp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gxalinynd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gkemmdxsh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gzcjcesut.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gdthbmgfw.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gayomalho.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/gyedkbaae.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gtvdbagid.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gyddkfzcf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gykrohhlb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gqvhokllm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gcflzgviv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gptcopzov.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gumcjktcw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gduqdvxdr.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gaihqdref.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/grlxleset.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gbeaufarg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gilpclxgt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gnbnghmlw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gkdvtqlwe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcjnhgozq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gxqlsobhe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gxabhhrto.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gcrwctbby.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gmgtzpyhl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gsvctxvms.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gcjuhwlvz.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gvqozylns.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gvlazppes.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gmzyjxtqq.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gbaflcsfz.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gjiubiqgj.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gvrrleghk.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gibrxydkw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gqqtllhdl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gvmipnkvc.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/goniclcgq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbjnggftv.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/grzfjcyos.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gbmzrjftn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/ggkrenbtb.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gikedcbxf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/ggpqpsnnb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmaomjjdq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtjafqfda.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grdzqfmwq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gskhvzcaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gzkcrapvu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gaipiulde.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqqjetcky.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gtmyowaas.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gccamjdzv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcrmtgbgn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gmjmfyyyc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ghowkndfc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gbbmxhryg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gjpmhnlnr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gmxgnttxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gzxbnajxy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghhzdrzae.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/genryyzeu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grudiudqd.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gexxxavtg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gaqjpabmg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghksvekyf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gecgvtmrv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzqfvelze.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/glikqwrps.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gvqgiybbt.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grkuanjkc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmswsqogy.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gzgzavlql.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gvyrjtgzs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gctjyjagz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gxqpkoydb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gakjyooou.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gvvnretpz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gvrrffrxy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gwawalmbd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gyzszwrdb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gextxwebc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gazlfzyvu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwxobityd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gpsdrunef.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdyxheuqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gcxbwjaol.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/golpxsjzw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gonewczxe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/glkhsxrdb.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gtaovddhx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gptknphna.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gwoudwukz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gwlggzlld.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gzugiuoqo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gmosxtaea.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/glsjwlndh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gegpsbxcm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gyxtqeeqz.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzhhkmtta.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gwrqfrhrq.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gbgwgthvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvqfybzrr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcvsibfnm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gkimkwnqj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gjscptatv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwhcyzyo.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/guqcqgiyv.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gqfulqgig.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkajulbwu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcchnanre.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnsrzmdxu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gflfvqicp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzqwauaug.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyucyfapj.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghrbggqio.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvkuigkew.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gndkjnlue.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gkdgqevcj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gukzonprs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gegdkslhe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gzdmgvruj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gqlfvewww.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhtwkqrp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gunjnpchr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/genydqmev.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gplzezkzo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gecdurssf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gepnwxcyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvvsbzm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/godcfcmwv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gihyxjyzn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gpylxeple.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gazkehijc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxuqrcvlo.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/glhoawxms.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwjdepbpy.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghqyjiume.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gcfiihsuk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvatqrhun.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gfkvlfosp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/ggawnhaxq.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzznuwjkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/glcqzpair.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gpfkrzova.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/grxwvlxla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpsaevgiw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggtvxyidm.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnscrmtnr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/guxhurxil.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyggwjfeq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqtliqmey.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdimvtxyd.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gxxssivnh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyppgvwpb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gxxvdxgge.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gaogszrsu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gohbqqevp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gnbutjmvb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gozfrnpzw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ghglpgqyl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gkbcypwjh.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gaoufsuai.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gapqvygpt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gvsrmefnr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gduycurff.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gjavepiaf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gwquealsj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gdkpiioya.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gcvqyekkp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gictsovqt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcdygnadm.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gstvcfaxz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gorscqwcb.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/grlxtlulb.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gxwykjnre.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/ghcizkbce.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/grkistknl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/guscfqryc.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/ggtvsrsnx.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gvvbnkgby.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gagtaltzt.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ggazyhfwn.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gtsxvhdrs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gknaejlun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gdnebotma.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/geabtokxr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gylnehjtp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/grptpdsug.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gvkvatkhc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gieokkfna.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gellictkz.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gpavroklr.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gkdsjzifi.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gjugtivgt.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gijlnpgaj.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gjivyvsxs.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gkmqfosgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/glufaligt.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gyqyfjkws.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gguwiwtwz.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gegicodmu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/graqzmtuo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gqlwbwheu.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gathoawim.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtuazqblr.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbbkqoqgw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/guiatzlkf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/glhgyrsej.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghmfahoux.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gfpwfvjmi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gqlwdfmnk.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ggevuzbse.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gstnqsvvy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gflzcamuh.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grtmozqww.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gysiuefug.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gszgbdtgk.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gylddiibw.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gcwlnqykx.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/guebnxhnd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjmirlije.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcbnwiths.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gbjbeeawj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjzqqtzkw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gionjijke.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gtpqbsvpe.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gosioxmdt.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/giowewzcb.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gwplpsqcl.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gzdghstvz.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gndjirryl.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghgiajwta.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gjxxmvlhn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gabypdfic.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxvipddlk.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gbzqvbaua.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gimggduyo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gqmifvdje.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gcplsmrsl.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzebughcq.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gryfprbve.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gwtdlhwal.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gwlciqifk.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gfvzhegbb.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gaavbuqrc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gverzpjzg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gpntztxjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/glehkmmcb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gzdlhdwvt.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/glztxtuzk.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gcckbtqyy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gjvhkefsu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gbtntorlu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdqytbzz.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gtmgguulo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gbtuxofoi.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gvqvacalj.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gintojqir.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gjzqjxsgy.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gqlmgthlk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gmummflya.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvhrptuzo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gqcgvufmj.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gxwufinsr.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gfugfqtra.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/glpwycbvu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gnagvjxbq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjiyzdqlh.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/ggmlvqeqy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gctmogush.sHtML


<!-- 参考信息 -->