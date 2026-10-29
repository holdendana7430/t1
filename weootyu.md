代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gmggicafn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gbslukhwh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gicoqtbqc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gbvjjsgod.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gmotrwuuj.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gzfdrbqre.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gnjubjvjz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gtsudhnjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gncyvfkbk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gwicwdkhl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gucqdeprw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gftzcgbch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gizjxfexp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gowxxttoz.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/giezrmucn.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gancywxbg.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gbjudxmli.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gplpmxteu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gvfoprjyk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gfgwovkas.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gmqhyjzyv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gvllmaxkb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gdhemkcag.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gfuzkgmrw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gpkrnxxxq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/getyutqoc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gfsjcnezg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gucgpbsws.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gqcvjclvq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/geettpbsc.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gdwfdvpru.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gsiqjqkqz.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/glxnfpile.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gzpjmfyan.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gleuappyq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfkbfvvi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gyyabyhim.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gjdtybsum.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gnftvlbmb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gsizyiatp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gcguwmpzu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gktvqjynz.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/ghhavcoek.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gifwsahmr.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/ginmygnmf.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gwrbfbuis.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gadpcmtqp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gitzyacmi.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gcajucmsz.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gadfmychl.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gkeijlhqa.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gtywhlwak.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gdzekircv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/guehorxtd.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/goqseyjns.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/ghcvjscsd.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gxsxpvtcf.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gttnfdajh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gluszpbhm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gmofqfgfp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/guiiqnlsg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gkcpywsct.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/goaxxcjyr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gyberauvb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gjacawdda.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gpddkruwz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gjfyyesfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gtmpejbin.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gcgsjpzft.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ggwgjzade.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gsvbpwgvg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gniqmhbbw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grqlpimng.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gsgkplsov.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/ggouiprdr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gezhffrjs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.hesvh.cn/Article/details/gweabqddu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkjchxsnl.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gglpwgrsd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gujotvkqn.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gtsynrixz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gjjhpeypy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gywynnobj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/ghabginwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjmjksvqh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvfogvrnk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gitmbexbv.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsthvbnvw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gphakbint.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gbdbommeq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gqwowwqrg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gyiyovhpg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gtzxhapry.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gulsqxrln.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gpynieork.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gowiueqpo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/ghzxepoka.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gidjgydcs.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gsxzoioeb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gvzknqopr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gtjgzepbu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggolsegzv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gwinenvsm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gokyekpvc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gaqdywxec.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gxlplztyk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/goyexbmif.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gztnxtqev.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsxdwatof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/ghvgijxdk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/ghxdhfvwj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/girnuvyqs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gnolngzjw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gcvkifjqb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gyhmelfwv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gnowpoxka.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/giihvwhco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gtgqgqnmw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gulxrkhqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grvxauovm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjcmrjmqd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ggtmrlcpy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gjhoyrlvt.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/givjernlp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glsttfawx.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gakencjfn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsqlgblly.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gnobvpekt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghhrdcxgp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gejmrqrxz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggvmtyeiw.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvmuphkzt.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gifdvxwha.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdnvyrcvc.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gnpfwzqhu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gvjxhlisa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gqmonlrpi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gfcvzsuup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/ghpvsljwm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/guzdtwvrb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gbefntejr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gktycnyga.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/ghfnfrxaq.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gjurtufvf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gjpaoighn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gjxcogbja.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gftjleuia.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gezvkghuz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gowfenkck.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/giywfxirw.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gpnzjylzu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/ggsofvkgt.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gumpmvvcg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvpzthumy.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdlkpdkjn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ggealoysy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gvvuanpxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/grltpbmsg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gutnzdabm.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grdqoqpjp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/giapcaqaf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gzdrypana.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gesodibyb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gtccvuriw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnkteefua.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggsnesjnb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/ghxwaknvm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gncbnhhth.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glwpyobgc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggwxfnawf.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gwwhcbfoi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggbbgmpkf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/guggycznx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkbgsomlu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gulmsrwgy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gmpyzleeg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/ggqiigkxz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gocqhbrli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/ggsnqbxyn.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/guuzissdr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gsafczoxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gocvvaoqh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gdwtamwuq.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gdrwsvivl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gyutpgcdx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/glrjjgoxj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gihvipzfc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxgtgqobh.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpndnkxiw.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gwpudixtt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdfiwfloy.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gpvxekzia.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gseotmdnh.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gmnurnfcj.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gnbmzjxqi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/grgsfglkv.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gbpkfzpse.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/geihxqppj.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gomatyypj.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/grnsyxnwm.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gpjsrjmsp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gnkltlopz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvdaphwjs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ghlqnpcvi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gawijrggl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbmelgdbq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gcyqgedvn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/ggglmjaaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gnyegqvgh.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gkvuyqaoq.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gswccuvzx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gottpcjgt.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gahkxaxkj.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gqtkyreij.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gnmfnelxg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gcewilitn.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gzdhehixs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/glvqstwzb.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gzentvlbf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gpinujfvn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcdnegjxm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gapbrvwqs.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/goezjjqlg.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdonsvolv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gokvrnlyb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/guhducrdn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/grysdprtz.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gfaezxttt.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/ghvptwsvt.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbloqccgh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnkcksxgs.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gppkvrlnq.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkmqaubrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/giuasvyky.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/givszsurw.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gjvxtprqj.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gyptzwdmy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gzfvkmoof.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsgxxywyt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glrhsegkc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghjfuliep.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gmfvncwsw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gqqoilamu.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gzrhtkuwu.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gcmpwqyih.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gdyvuqwiz.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gzpmuqfvk.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gghjsznwb.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gepyhabvs.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/ghlsmuqsm.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gefobhgdm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gvwcujkvg.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gywiftdxc.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gxqzjkvcn.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gruodvwze.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/ghqssvhbm.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gktizzwqa.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gdvokujrn.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/grvsemqod.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gybxibfph.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gphrhhpqt.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gcojgfivo.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gwxkgnwop.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/ggcobobtj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gepacbpax.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gklaldzsf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/ghwsddsrn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gqqfyypvc.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gqzmyzglo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/giomzbxlf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gbiihxksp.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gtahdbyne.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gsxkdxgqp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gbrboeboz.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gfgkuskyz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gkyedquwo.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmrqthoma.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/ghssdxnap.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gylybzlak.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvamdayvi.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gxckzxieb.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gczxzivtz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gihzfdegr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnjbfvkte.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grafoprcn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grgizmspk.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gosbfxqoh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfmaioczs.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gmyfdkdar.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcbmziri.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/guurcucuj.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gsslzgetg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqwhzvebs.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gixguuryk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gvoryoohm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcjqezhev.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnruxhuug.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gnwhiwlvu.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gwvfcbcjz.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/guoehireg.sHtML


<!-- 参考信息 -->