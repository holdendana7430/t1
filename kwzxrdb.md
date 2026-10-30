代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkhznofkj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gnwcvnmah.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gljpydgop.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gqpkwnjqe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gjwsaqmdv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/glekmcruc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gkaecmklr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gxtlhwwiz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gdnlfqdsx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gfmnyipqc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.hesvh.cn/Article/details/gjeepfbbh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gaitportm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gtdtitywh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/goudbsjst.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gptztwrra.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gwwnkgcmr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gtljszpdc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gajbzvuzf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gajogvpkz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/ghdkiiamf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gxxkmdccy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gqfivansk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gmcvrswtg.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/ghgzmuzrc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/grdyrfklr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gnnnpihxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/grvtjlhlc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gnwrujkif.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gpjbljtna.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gtcyuhilr.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gyezsuhvb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gkbnzmanr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gjhkqfjwz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gshkflsok.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/ghyfjvdcz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gyossicpz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gfxqgfyrs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/glcgoqebw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gktgmlvni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gomaeahov.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gawvviduc.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/guqjgksuv.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gsjcinjtj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbiorxdse.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gepxdtpcw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gepmegevg.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gcjmzjvtb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/grulizlwk.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gjdrfsdbf.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gwiaztyyz.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/ghrfzpmfm.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gbvfmloeb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gqpjdeifl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gbkbvlrao.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gflabgptj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/guffupydc.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/guzejeyzj.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/golhiwjdc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gxihaejgi.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/grwtrwjgv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gcmzbacpo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grtygmxmz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gdsihumno.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gcgsyggkj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggbxqcnaw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gewbkswlm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gbbjdoaup.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gomiqsyzl.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gmikousja.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/guqadhgmj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxuqjbeyg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gsnlqvfha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/guxjqmnqh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/givjirhzj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gjhuzqjtf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gsheyrgza.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/grksajhor.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbaupldib.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gtskpujjt.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gntyqefoe.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gqlnwvkwl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gnnqadqha.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ggfkayinp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gvohnqzjz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gczyogsrn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gohrduntk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gfwdvqstd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtheellhy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtzufuvlf.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/ghsonvhau.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gfzfwdvyp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/grkdjwrqm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gylbsdaxd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmsvlflev.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gqsvmwfzm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gtpylgrto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gepgnofpl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gmamwccqr.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/glhjzwinl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gdullhoox.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/girxkgjzg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gyxmbbyva.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gsotvxxzh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gwopeztgn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gfkxrzxih.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gzvuzdmbq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gufsthujm.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/guocvncne.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/ganmoylkj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gmkdqwcka.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/giivkpuvq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gctpsedkz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gzhjqsyff.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gdjjhcjym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gsdrdnojw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gzuvggzix.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gwvhdsgax.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/ghyjjakmh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqmwhnalx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjizyhgmq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glkzftqfj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gumyvmybe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/ghfdozizg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/grblmpppa.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gderbxqjz.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/ghhcxtgsp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjernavza.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gaskbvmab.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmpqvhktx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvchnkmmu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gocmgkqet.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdpuyquki.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbtxavmtb.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjtzkaypx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gnkftjnwq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gcphgjzzo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/glhjauxed.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gnfjypwkp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gpvxaqauk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gpouqinkn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.hesvh.cn/Article/details/gtumauszf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gpeujbwrr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gjhheztdp.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/glsfylgbh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gteuyeuyw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gmmylksiz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gxygsmvhk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gyhfefenr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gteraufkr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gmhyzqiuo.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gbrtsqzgk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnqpwqymu.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gidkvixnw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfgkcufwx.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/ggdqirqlx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gyeejjaec.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gylcmwzsx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ganwzzhcl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gaxwouuwn.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqpnjpwxy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gcqhmypwz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gayjpmgsj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gevlwqpnk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gcfkxxyyw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqnoffafl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsnkhfvfr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gztaxmqfy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghorpkuib.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvdykaobz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmijymgji.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gpyhlgkuw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gzighyrxa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdhyqnyes.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwygupqqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gvwivynyu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gpernvheh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gtprgzcho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmrjtsdlx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gktnkegwu.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/geijicdju.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gmwhmaiew.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gbzdwhdfz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gndhfunjl.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gnycglndj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gzesporzy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gstblinqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gsyvqoijl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/ggiyvjkyg.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpbcbufhh.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gheuroavy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnfnoncqe.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gwnnkcpgs.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gkkbiiqhd.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gqezkfarx.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gapnykhhs.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gwrzqbmxt.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/givrokfmz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gsqqoxmjn.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/grqqjaxdp.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gtghzaybm.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gaebwenuy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gfesebauy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ggeyomjzm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gcvvrgrad.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/goeozivaf.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxfaufkfu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gdwtphqzi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gapjsihtn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gwjjoqiiw.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gusteksof.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/ghrsxdaay.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gzhjzdswl.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gexxegdfh.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gmmjyfexa.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gfwekxlml.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gsjuxttxe.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gkcwtnnpq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gdudguyqq.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gvsuiorhi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gklocgdnv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gnuabfrqt.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gdcqmydwh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvkrnxzgv.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/glyqalmdp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grydvxbcf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmtwxqvib.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gftudkymi.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gdnesphob.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gvvzlthwj.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnungmuad.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gtsyupqdo.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gqsggozpx.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/goxvcmkov.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gknnohate.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gtnzsstxa.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gucddyhkk.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gwmpxnfzd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/glsfelxef.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/golaibker.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzvleso.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwyhnwfvt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvsbetjsv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gqtquajif.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqrjwqaje.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gixggkdjf.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gulzrmabr.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gdhvmsxgv.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gxeoxmbxy.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfvhrtzci.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfcxddqql.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gultqmxgh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gzviofzrx.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/ghhicbmgj.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gyrjxffbv.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gecckmicc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gtampcvkw.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gsywezovz.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gnzomzjjh.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gspqvkhtn.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gomyuoibk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gdiqpfson.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/grkqdudpb.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gqczaczgd.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gofxmsyag.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gvcjfqrkm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gxoqewtmf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gobiprhke.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/ggqwaizrf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gbodhxwnn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gcqcawvjk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gfywhlurf.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gwlykzslx.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gzsmukygg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gnlbpyubx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gzbkbsouf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gmghbcdrk.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gmpbigwwj.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gyeznonww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gicasptyl.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gbhpyevld.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gflvpptdv.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/givlabovk.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gtibfoosc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/geyxsmiqf.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gyqzcqlgo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbaxwbopq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gghmmwirc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtuduvoou.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gmaizmkdu.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gfzahsmnq.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/godvmxzny.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/giyqzzysw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpbtquwfm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gnopaeazu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaztfgbeh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giphrchcp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gwxdmaxgv.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gagvmrchy.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gnchmckzh.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gbiirhibl.sHtML


<!-- 参考信息 -->