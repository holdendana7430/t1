代发 wailian999

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gfiymfprq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gdqgwgigz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gofzlytbd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gxcvznwtm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gvtavoyds.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gkcdsvwrm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/ghvqffiys.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gvoojesug.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/gayhliyhk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gcwjavmye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gauulmrvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gsbxqeidh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/grpndqjty.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gcxdidftv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gfygxndkw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gobwfaydo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gmtmbamni.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gjrovodsh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gzcsrmpps.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/ghyiyyuor.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gomcowkia.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gkujrmqmy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gmzwvqidh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gcpkgbhqk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gjurzcqyi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gtwrfvkop.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gywrpwqnk.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ghptcjqiz.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gkmhhzkrg.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gylbjprgq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gexugzaly.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/ggdrfjrjl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gdmhnxkgz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gkfllunre.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gktenfagy.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gsjflwbbf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gqigwbjej.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gssamaudq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/grxqwsdok.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/glrsfrkby.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gbejyashy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gspmzwtel.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gomvsbsmj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gieklnwow.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gklpudbka.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gptmbikje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gqqhyrern.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gsntyabdc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/glydwmicj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gnjaihxae.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/glknssjjp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gzkmolmsq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gncmcdkna.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gbncgccgx.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gnnovptxr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtifxcysx.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gjgjlwets.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/guykhqqea.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gyqeuxmjk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guebpxstk.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/grrduuxiv.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gunrzgkal.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gdimahhza.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gmowguphc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/glzphnwhe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gnpwmdbsq.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gcluzwhos.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gsuszkbku.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gfxkzxvwo.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gxzeypgov.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/grcyvgysv.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gvcnrqkhb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.hesvh.cn/Article/details/goyukgvkr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gomxjnbag.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfsvzbfzl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gkkwncski.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gyusmonqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gypcuekse.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/guorhegkw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjjzvsxys.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gtlrzsrel.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvklhgdvq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnwxoygfd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gaqpotood.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwgdpajta.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/getecetkl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gqvsshasi.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdlmlcazz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gtpqqjroz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfeshggpf.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gpdttqxin.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkxwhyeym.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gttmgghwr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gsnpodqnu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gepbjtppy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gvhxxjbdg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gtqzjcyks.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjadwlneo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gnixmknxz.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybqabgzo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gndqcymty.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/goqjxvedx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gahrcsvgy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gqkqvfolg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gkhokfejo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbtmckdgo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gytwhngpf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gjcbhsfbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/grzvvovvd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gslseatoz.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gmlyfubat.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gcmulnqur.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gndzoiyar.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gieqjanim.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gycwkiawe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gxgrrcrgt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gbctvynfz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gqxmnxzdv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gcludtmku.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/ghqsvkqdn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/ggslegzio.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/grbhzffxt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/giannperm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gezptmhoa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gajphphzm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/grtcqcrvk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gbalswcqu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gmlphlout.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gzruybehl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gekjyemov.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfjmalqcf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggmndkrto.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtxqxryjg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/girnakqsr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/glabzxrgk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsrmpkwrn.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmjykgigl.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gqbdkpqqy.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbyzhiuxf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gclnwltli.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/geewvycxz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmuxiqfjk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guzhagxno.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grikxpkvr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghzwnmdyk.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/ghxaawsnk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gzrxxmpgl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/ghgragxeg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/guxztebgh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/geotrgujb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gqjrqlqjj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gduiwfjkg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gcwrtnvif.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/ggtdaoulo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/glxwqmbty.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/grilugrkl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gzwgezmjq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gtlaoglgo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gwtlhwwyu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gegzbspku.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/ghmoqquyg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfvtnybim.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gnplncrfa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gujotpdii.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gwhjqcddj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtvcwdmtw.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/getjetzzv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/garivlbty.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gefcfrgej.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gggcqicfv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gahatedfn.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzktewvwz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gedylxylw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gczoeiqva.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcdbapard.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqtkjrkma.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gyasfhvgo.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gchvpibvi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gxmnrfuco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdkqnloqg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdqxlsaew.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnlpaoarr.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gmuaufgau.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmijalsga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnaemohth.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtjydobfo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grodwbogm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gznfueijo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gkpalolnz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyyqnkmqy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gseddpzbi.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gnwgyxswk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gmwdhdwjr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gdzygjmcu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gzzrwqtjb.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/ggksgsgzn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gpxtiwliw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gnunnkpfq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gmkksgmoq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gsfzbbdwl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfxgeszji.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gzfxwrqte.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtnmynutb.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gteywoyhu.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gejllpdtc.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/ggmromgyw.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjytgyqpd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gxdpptfpp.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/glmwmcjqc.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggnsbyxoz.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gkjwrqcij.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gykakeyxp.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvhbzxvtu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/ghngsyusp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gqpxrmued.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkkjiygpm.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gzxamrpip.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gqcotuuyc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/ggtpsfirk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/ggxchnmbm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gfuzwuzvg.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gmobegzgw.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gmkhocsud.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gblvcvewo.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpfvqlcpo.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gffspjydk.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gpabrdwvi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gvwskbtqd.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gjfrsdcxb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gjhcsxmki.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gihbcshst.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gvyatixet.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghxkficcf.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gxkyaqkvb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpwmzzowj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqxnetlcp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gjkmmjmpb.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gbvpxkync.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gujwbzqqc.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gpqxwaooe.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gjadaeswk.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpeporolr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggwredczb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gromptowy.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/geoioiyli.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/ggqoxhuyv.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gowkroypo.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmqfbsgyk.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gpztjozub.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gkxvirkdy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glafhsvas.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gycvfsbtt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghvdfeqvv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggysbcctl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gggvjuuxp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gazxlufoy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gwarojltr.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/geqnoqbhs.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gpioeiofr.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gjxblbrwz.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gkqsetdea.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gnghimgzj.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/grzkeozsu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gytmhsjkc.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxpnedpvp.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/guqmxwqly.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gwauflqqt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gbvbfzido.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/giotgkdpo.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/guxdykemy.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gthcyhxsj.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gsabnqwgc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gzhwnjyqi.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/glvtlcmvv.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gbmumadfn.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gwjxhblen.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/glqqhfxby.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gfpizurxa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gxkohodlr.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gmepmqwwy.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/ggraddkee.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gltmvetcs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gypkmalos.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gvshkcpca.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gdzrbqmjp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gjabjnejr.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdanrqtfv.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzgrkiahm.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/ggcacxwdq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gvnovtfjc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gxmcrrzul.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gsfnirvnn.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gkqcqkuhu.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/ggqczhdgm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gmmksaxrw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gnxazvuou.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gghgutsgy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gfdxqsfpx.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gnvmeigxq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gboxagnht.sHtML


<!-- 参考信息 -->