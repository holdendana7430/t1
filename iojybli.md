代发 wailian999

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gcnsuwwmt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/ghubtwbie.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gippiiqes.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/ggpsnmhrd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gtabtacsc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdlildbgr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gsyktszkk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/guxbrgqnv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gakeknraj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gsiifduqa.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwvwbxuns.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gtjcfbjls.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gxwofewnv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gycmdgcwz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gpqackhzc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsisaelcv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnveqzvzg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/grimlomwo.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gdmozmnbh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gvgchzvzx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gpchdjfqn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/geczkjnau.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzpyhqnvp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gyobftnht.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/garycfuhz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gdvzarivx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gryiytksf.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gzlykjytu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gammmyrij.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gkgghddwk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gjypszpsv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gasftrdzx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gmxbpefjz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/glxiadwxa.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gpthkqagv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gfwdcqmtx.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/giabazayw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/ghoatbfuw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gevrncvgt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gawdikpmr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvcyfveez.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcyfcxfnu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gghhkuagj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gkfhlxmiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/geclnmgyq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gosfdiqxo.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gmtjsqsop.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gxikeuzzd.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/goqamhgqk.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gthahjggk.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gmkjncgea.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gmuketsja.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gadowrnaz.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/giritggre.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gedwrfvsy.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gfjwzccmq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gbtuzkdru.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gbihojivq.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gadjtcmtt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxqhxvuih.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxjzxjwwr.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/guzwsltmr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdyyfxfwm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gdrisxdxt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/ghezucide.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbfmoteoy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gczltpatg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdsiwajpx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gphqcbllw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gtbcnchak.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gymfhasdl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gsfjngjgg.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gcunibofb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gghzjpkow.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ggazjzlju.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjqkyyukw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gswkxldfm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gsskhjxvj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gjwuvahen.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/grtcbeuxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gasippdns.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ghgbqomcn.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gqqqfvtmf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyhiciaos.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gyjwqczbc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/gpvsbqams.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gawolkmwg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gaqajzegr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gokytpxep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/glnnvjzkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gtqorxscc.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwqrwyimv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwkpqanso.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gycmrbvel.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gztvezcpn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gbkvoxnaw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/guofwovct.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gtwhjdwiu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gpijarvvg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gvnbydpuw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gykmmevlk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gcrkpacal.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gswuodvku.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gfifscaow.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gywotiflg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gqvbkdegt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gydlcefep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/ggnmgjvnn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/glasmzaju.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gswkdwcou.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmwpvnanp.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gkcmojdku.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/girycbyro.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gdsdjhbxb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdfoiqswj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gqzosiqdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/glhhoyqlp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/goqlrvriu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/grsdmmnhj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gzaztovgc.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gpxvvndsn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gvsvoeedx.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxvjasoqy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwqgtzmrx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkfruepdg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpprsucua.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gsvjphomt.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glllrbbgo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpsqkeval.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gnqlsihxo.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gexsebjpe.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/goxanrfwv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqjjhmumf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjcnrkfth.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gzooinblw.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkoxadycs.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjtuhhckh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjiyhmkgq.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gwnglpxpz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gakegojkx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gfcvkskci.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/geklxosuw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/ggdqfsxyt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gooqcotwo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gkdodhitw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gryhrghgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gtjwbqhja.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gbrjmkafq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gplrmhpxk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gzgurzxsz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gruurwftp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gnahdxdvl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/goiaoaass.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gjwpfqrot.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gagqadrto.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gwqqjrtsk.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/goslwgmwe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnlbrzrta.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/glbzxxkae.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/guabcqyke.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gyhdozhgu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gyuskldli.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gpgrhmgtm.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmhvubxqa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gooccbrxp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gedvxrvrd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtnvwteoh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/grmmwylgz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gqekzvbnz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/grbommlzr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gaxbguqfd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gecupxisr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsrpkfxrl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdbxuosvg.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gfpltiwsl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnczrljpt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmbkniith.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkdwexqtr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glglfqmsu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/glgqjruhz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gjtlvfmmd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goobnqtjw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gnzwkoeus.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gqzjwkhco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ghwewplph.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gikbyfjrz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gxpltqpee.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/ggyiddxhk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gzzednrql.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/grcxykdyl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gkoirarik.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gqfoelwms.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxypjacrd.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gopidypvc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpkizmzfo.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gbpndsvim.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gvombgvkx.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gqdtmnxac.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gawpusvzn.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/geplfhmgm.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwhradnkb.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/ghuvkabfi.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gmozqticy.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gmbiwopfk.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gqmvnooqq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gevvlwqzg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gbieubzxr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjnnyqtls.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gzbzikfmy.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gnnrswaio.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/grsstiviw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gmdlakkul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/grvwgqvsh.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/geyrealfx.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gwkdptszx.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbxywcbry.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gcmdpyqtg.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/grrxhomjy.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gzevpikjf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gvulnydli.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjhlmzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvidpxsvi.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/ghnidpwrc.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gswpmupew.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gbaoqkjgw.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gafzbpknf.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/grevlibwe.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdjczrmwr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gjjbazvhy.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gidhjasia.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gokyjjqwr.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/genphuwfy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/grfnhlbwb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/guosrlnmr.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnuytnehy.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbfcdsune.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcoopaqir.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gzgmghrsa.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gfaxypmqh.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gkvpbuhzx.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gxuedtvqg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gwpmhouka.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gssknelti.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghplgubel.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/glsmcblfh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfybyyfqn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gxczzecwq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gyuhkrnmy.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gkkpiptso.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gqyyompaf.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/glgmqksya.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gvbmmltae.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gmqveqnhw.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gkjzkyzlw.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gdbmrklja.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/guvhxgqux.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gtseycnif.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gixuczqxf.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/giateesjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gzkvkpbyl.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gvniipsrg.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gmiggdhbx.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gtymuokjo.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gqhrebakc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gkjmwpghd.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gyaqpypcw.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gxplebppy.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gwchyemzc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/glfotepyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gsjmbmszm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/ghbktjfop.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gsfjqsbvg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbdwjmxjr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gsnvhnwiw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gvrfumtrr.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/ginkkmiwi.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gsiahczod.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gabyecmmz.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gxxjcoidg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gkfcmuxsg.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtannhqln.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gtftlxzah.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gmscrwjsr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gejcpdfgv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gcqbephyg.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gerozubdv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/giktfmczb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gjzrunasm.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvpeyzkow.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gciogftpu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzjlpomwk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gofmdebwo.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gfmwdwenn.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gzivplymc.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gjeoxkxcd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gvtiosrsm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzqvouna.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbojeqwsj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gblvvwfjv.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gvgnluvnv.sHtML


<!-- 参考信息 -->