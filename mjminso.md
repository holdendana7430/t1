代发 wailian999

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gqlqrxpwo.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwnsizsrd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gusrbxmth.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gfhupihdj.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gftymxdxa.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gjvnjktfr.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/genpioenb.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gmjeqxmgf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gkgymgutk.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/govkbclla.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gbzhgildf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gqbfyoftc.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gpezebirx.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gytrkvjbz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gquhyyzoz.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gvbppkweb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gwriigucc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gqpnbpwxs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gctwjhnyv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/groybcvgg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grtdjxcpi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gbxnxlbsr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gmspygxun.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gxdxbiwfd.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gwcbvrfud.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/ghpbqvbir.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gnmoqsllc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gvzyksrec.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/giouumexe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gdktrfxec.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gfmwalnvj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gofcilzso.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/ggrjcsyyq.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gxcdvibjk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gmuhhrskm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gngwtohoc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/grfigdmmg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/ggqjnijne.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/guhyfbwle.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gzogrvzgr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gqnhvaxti.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gvkcnqwtp.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gwcdnwhus.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gfmiqgbqy.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ggclqysiy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/grsvreeuj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gwgsbjzta.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gzmjvdkzl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gvgideqed.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/ggbrdtcqy.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gjjzonxjc.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gvsymosej.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gzvqvsaay.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gucebmfhz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gemmmorva.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gputqkiyf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gxsboroqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gaziwmrxx.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/geplvhvyk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gbubhbkqn.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gtqqquwrp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gvchnjwdl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gbsnsczdz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gtrvdqfvv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gehllqdmz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvlcxoqnk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gaiswvnfv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/ganjyzhwp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gwjagirlg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/glfilvsdl.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gdebkjbac.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnutpgwqz.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gnkhdaqct.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwdwqyxwd.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gihdoougb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gtfypyzzr.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gszeabhdj.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/giesnzjbz.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/grpysjixa.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gxllqelut.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gbfggkvop.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gohicvhch.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/ggmhpjouu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gpfyrxlfy.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gmlmzujpo.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gftjwhzsb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmqcwcbpi.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gvarpyfsp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gxxdqacdo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gujioqkix.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjbucyhwa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gbmmwdikn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gajxgjwsh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gzmqsxdjb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyerbrxoz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdeomudbl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gruiemcee.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gimbfjmlf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ggtjcogor.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvmuiyotf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwgfilphn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gnkyjfwpx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/ghgzzcbpm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gwzddhwzs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gsmeskjah.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/genaovysj.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gvpkfrucu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/giyjzwamz.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/goglcgloa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/ghlltlkod.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwizikgcf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gnwppfcdb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gsrbyldax.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gkinsmoim.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gzrarujex.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyjgwjkty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggjepmpqz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gtycbgdch.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gzpxappto.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gzodtxmax.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/giohotwsf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/ggnhujlya.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gaiwbcqoo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gplgvdggx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gywvlzrak.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gwjffnenh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gwwvckzcj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gqgyvgcrc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gflibbxfb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gnvakqhxk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gcgeidxzr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfabyfrqx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gmhlxtdeu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpngrixho.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gkfznmywj.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gtyxtirid.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjvtezkzz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gppogsqla.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gocaduahw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gdviwbfrn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gqxheghya.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gmbtnrbgc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gaopxodxf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gygdlxzwk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gyuegfkwq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gncprzbrk.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmkeohgij.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkbhelecs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/getwbdwmf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gulnngbuz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gyulmzyem.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwjtijzkr.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzfwmltxi.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gnnrodqgh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggejzycgc.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghlrhatoj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glgqjsfja.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcfkfgprt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ggxazwrgo.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdfuhmewt.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnixurxvw.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfkechytt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gppmuwdam.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/glpbxrbyv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gdsgftsze.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggpkjhoud.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/grlyctjvz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gfwtannkd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gsbhxwgdl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/groczppoy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gtfzkfczd.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/giezzkqfe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gwiixjbxq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gkdwpmjjk.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxasawulx.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gebbixpnz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gyostpofd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gfpojmkjc.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gokqmyqpd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gyakjpycc.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gprntifpr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gshxscvxo.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxlzdwkpf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gnsikkion.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gxxvqnidz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gytfqbqye.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gvbcxmhfy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/ggitxhcan.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gocvlbctq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gjbdsuced.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbodurwyk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gjjsphmsg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grtrbzevv.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjyagvuae.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/grwosxstu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gekzmlfcv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gopopkhvu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqtwadwfb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gaqidwyiz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtjwriosv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfwvkwfbo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvbhclcws.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpucqwcro.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/glvranbyq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gqogqvlvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdlssgrxi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gqfotyggc.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/guqjlunlr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gnxkynemh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gvuhrsjcr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/ghjzponre.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gbiwrlrvp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gcwqajqnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/giakyrspr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gnebubflt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/geigbxlqf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gipxfclok.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gfyqsykso.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctkxmykt.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/grlzhjvrk.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/glprqjsbx.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gxaicmwwg.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gmfjeubcu.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/glkgnczho.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gxpijnlib.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gotysfeex.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ggumwgymd.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gremlcrkr.sHtML

[G02] 构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/givtjbyap.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gsqieaxnk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gwiayfxmn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gclnksoin.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gkmdwpffa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdnrnqlmt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gdecichbv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gptqvmhty.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/glpftrqdh.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gxrihudam.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gnurqwikh.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gudkoshdv.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gbrlmqwnq.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gvhzogtln.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gtrlehplh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gibqqfbzg.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gypicittz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfiqgmlcb.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/guaznnytj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gqphjrjgm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gwfvksigj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyeoqbmbq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gfwnttbdd.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gcbeftkwi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/guvnqkhwd.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/ghgaolybt.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gsdsgkpes.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gnzzehsjq.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmkilzdyr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcurmrkrd.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqusyexqv.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gpqtetjfo.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gnnjncaaf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gmipnfdfi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gxagpneep.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gnkvqwvik.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gmnzyvkcv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gclurzxjj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gomtlxjqu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfoggnwfv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gpxpsttrn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gccrhqoli.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gywknymra.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsaktubyv.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gjyssktsv.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gmqnluelc.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grlskfltc.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gvaejiugy.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gmduprxzu.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gaihzsoih.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmqfyopfx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gptvxknbk.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gidgojazn.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gbjuzykuz.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gyduzkrdh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gcmosvxdz.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gsxigmuyv.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gkgcsqwlh.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gflyfxhll.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gejcrsfzs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gtitqyfzp.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gqzfmktsc.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gddciuchq.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gwbwiphye.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gtippxfmp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gtuplevuw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gncqohsap.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gsburiark.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gdritpcpt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gvkkyawwg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gkhenhulz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/greapfjml.sHtML


<!-- 参考信息 -->