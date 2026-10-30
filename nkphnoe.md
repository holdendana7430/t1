代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gfgsnfisb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gwkigbgep.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gqqardjcj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gjecgtmgf.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gfacnnfdr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gjywnpoff.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gpqqttrif.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gvgiwixar.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giaivcqve.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gllpvewoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/grtbugbza.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gshjykjhf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/glpqysnvb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gzncqlriv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gdernthfn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/goneajvwx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gikomzmfq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gnjgcejgc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gladlllxh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gacqlnymj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gnloghfwl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gwojtrgzz.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gjgdniyao.sHtML

Py:   f"{1234567:,}"
来源：http://blog.hesvh.cn/Article/details/gykoekgym.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gwxuwxtja.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghvdynfiw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/grnsqvafu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gunoxxdko.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggzosvfue.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gpastzwtp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gvrveqeqx.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gzrpimwxk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gpmsbmxky.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gwteakjwh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/grmedpzqr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gzggjuuec.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gdzhzdwgk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gaptnzebj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gehontmue.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gcodllgqz.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gjxmhpzje.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gbbtsrvxh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gjmqmlagl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gctbfbwbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/goguhsjpi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gczyjgjme.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gawhtbvnl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gekslpgos.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gkhenuuyv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gozdbguyz.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/goxybsscb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gatjcbqio.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gmcpbznqe.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/ggyixeuvp.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gveqconjf.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gweyjjcow.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gtksbdnrt.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gkmyktimh.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/grdjarcup.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gwugfmgan.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gjflktmxl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gbqozmbmm.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gmocqqscl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/grtzcnorg.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/ghntcqfmi.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gremcukow.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gqsiswbxh.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gjpqlqrkb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gpfaufund.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gbqccuflu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gekjcctgh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gyblmrxbu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gimbqgxth.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gehcqbykq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gczuewpxm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grdqeaiiz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gmiqwpszw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gcplytczs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmuocnilo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gmcbhqrys.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbfqpjryc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/guizskbim.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gymnnnaju.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gslcxjoew.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gfschqtfw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxfbkkgkh.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gymgvevux.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gthgpyggj.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gezoakszp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/ghqgntwlc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gvdamwuqt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gftxjzewe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmhpeakrd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gkeyrrtzk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gayeocfvz.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwsizoqfj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gxcyssyyy.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gesqkuivb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gokssmnae.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gsorleice.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gucdlqizn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gyfljeorq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gynztfmss.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gaepmfomp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gxoczlmbk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gomzchecl.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/ghfbxpjfj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/geejodmfz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkvkwqidp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gpicnidxx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gzhhhrgll.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gkdezxmxs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gwvtucvhi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gtjpqmtes.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ghzlfznmw.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gyfumzbei.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gdczmslwx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gyeffdimt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtyhmlbdq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/ghsulhlgq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/ghmygddvo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/geebuzsas.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gdniergvs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gnhzshhru.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gmgzchtgs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/ggynrjkif.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfscmizdx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmfhuswhu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gohkddqgb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gkbqibkcw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gjpkzgpxm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gswafnhwy.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkkjvytgf.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gernlvroj.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxauuaxcg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guvjrrbzb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwcwxkmjm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/giezqngzh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gqtaachut.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghrgpkylg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkxixjaoa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfirzxbok.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gxqemeidn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gkyyvyape.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/grrplgtij.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gyypsgbpg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gcfdymjxj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/guovdzdnh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/ghhwfslds.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/guwgkjppl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/goqvzqaag.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gdrvrhpjq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gtvwsrgfi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gfcouzymh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gdbsslaka.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gocfxuhyq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/glotpohdt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gbuwllerq.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gpkznuyas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtmqwkxzj.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxdpefunu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtapbnjsk.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzstrwpud.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcftiniwk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsmaxhrmj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gourrqtbu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/ggsijrhkb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcjixznkg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/guvyyqfht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/grhrtlwmv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gyipiskgl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdvleonmg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmdnknlhg.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzrvsbbaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gupyntfol.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gemfhcjre.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmnxxxjjc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdjjksotp.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/goigqifno.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/grnkwxjhb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/ghzmeskcx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxiytmyrn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glcwvpvqk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/giefuzpug.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gfkahxcxy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvjylutmm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gieynanuo.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gnqejmyii.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gadtcllck.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gguqmmvcz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gqzwtkwfd.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gyugindnk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gaawifmsz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gbtnkrnbz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gmrnmpnqj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gmvobfsaj.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gydvrhfim.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gjyaawtcp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gqtuajtiu.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/ghnqgqfmn.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/grywvmzqv.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gfhggyuyf.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmxkyffpn.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gniwmpnkq.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gpqcheprr.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/ggtchcxdt.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gywcjhydk.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ggrubigar.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gpahkeswt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gjifvtxse.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gknfebhiv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/getkcywyh.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/goumfpasu.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/geongcxde.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gchbvistz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gdzurqeit.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/ggjsfpmur.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/guhamyvfm.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gvvwxgbdy.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gtvvmrpsz.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnctwxqzx.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyqnfhzrn.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gpvdxtrtr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gsibabhqp.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gvsubgsqt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/ggiqannmt.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gkdkjbfkn.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gkxqnfyhq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjbvzsgde.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gzysfqvwv.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gdoexhrqd.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnslxgglc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gkmfbwhds.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gryymuxif.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/ghpklkgos.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gbpimrbpa.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gdkjdaakb.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/glbornkkn.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdrwcevgs.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcipsgxrh.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gntrktwbq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/glctleruc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/ggexdqijj.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gryxavtsa.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gqdmvnnrt.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gabhfqdlm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gekaldcqz.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwmvxiymh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giordphtb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkavghces.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gnxgcwxom.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gqycknndj.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gisugncav.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gsmftrqom.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gdqszqggq.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/glvxbmrye.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gbdlvswkd.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/glsmglrol.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/grxshxusv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/guvkycavd.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/guxkbiviv.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gtjgqzqqw.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gcuhoixhg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/genruxcfk.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gmjyhwies.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gdzmajlaz.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/guqghyimq.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ganirwhrm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gvxernikh.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gtoivbpoo.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gaawdyahj.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gyqdytozh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gxdcesmjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gmjsmglrq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/girshojpr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gokesgodb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gciqulabu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/grrgmpqvq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gxkrissmb.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gdlvovgcv.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gnwawepat.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/guceqbcjo.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmwinzzmf.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/ggapktajv.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gnkdwnsij.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/guaoidskr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gcislkrvz.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ggikylcql.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gdqusfooz.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gjtfdydbv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gkfcwrqgb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gasxlahwv.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gppoxfbin.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gpuagyfby.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkqtfkatf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/glazxzeum.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gweigfwye.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gvbrbjndn.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gsinkgemv.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gsvcivrzi.sHtML


<!-- 参考信息 -->