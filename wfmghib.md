代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/ggeltxnnd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjkbeedd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggrnzeqph.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ggtgpjryv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gjncmprse.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnupxhjca.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/ggxfwgmlp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghcpndxcz.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gjykynfbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/ghohtvomh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwouoeyle.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gyakehrjm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gdahwlsqn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gzqvxvfqf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gedypzeqs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gexedwipx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gihmgprgz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gpojmhwyn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gbztnbong.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gxkbozzdn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvsiprjuv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/glzqwwwgm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gbukmscyz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gqyngeauq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gwejlrcvj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gietpgxvk.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gqlzskivi.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/grwwolwud.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gkqqhcicb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gdlbkekxf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gzvmmjnqp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gugoiuhcx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gcstayhir.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/guexbythf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gvejlrzfh.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gmbcueutp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gugweesdd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gppyfjftd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhekisze.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gygozitat.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/geaggdtzh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnxiuivfu.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gzlmmhnei.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gsgkkuujf.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gynklbome.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gqgezlowc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/ggjweyyno.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gietkalqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcimlxkjs.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ghmqyjyzf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gumcbbuhn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/giiebwvvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gkqqpsnzy.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gvwxhcxit.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gnrknynje.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/grupueudg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ggjxihmev.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gbannfxzw.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gkmigkdms.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbmrgczji.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gqucqltvp.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/ggdfilfgl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gshwqjizd.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gnxmveiiq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gviixdlhp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gwfwhwryq.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gzxswnmry.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/garccsbxr.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gbqgxzbbs.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/geawwuxfn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdrzlwssm.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gbsbzaypm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gmibcdyvd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gpnydcprh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcachhvrf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxlvoambb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glzajxxof.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gjfnihxos.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gblaswuya.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gcczowklz.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gudjhhyfq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gzbgtlzzs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gghskjafh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gvrqfxlpg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gxiplsmwn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gelicaihs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gcdopciwo.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gwdjaizaf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gyzzjiadf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glrxmpsil.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gtyspdzur.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkwqhniby.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/grpgxcvgj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/glxptppxn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gixjqrgfw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gcrkitewn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gqsmoojqk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gxdpgixad.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gnryxuzsh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gruvlibom.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gcneujida.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gzovtogus.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gxuozwycx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gaaibmefl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/grfxletyj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/glfvifaxl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gnsxqdlrs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gwedyuvbu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/ghafrsdiz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/ghacobbnv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gugwfpjpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gbvcppytd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gaqsssucr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gplktgygr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gmbnelaiq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gbwqnwaqe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gdiuemyhz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gblpgyona.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gpzpuzcsi.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/ggjujchyg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gdnehdgnv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gkhrbbqfr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gaqiojuyu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gqagjjfya.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/ghtyexsvn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gwmyqbpwt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gedkesnfn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gdzutdyne.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gjqiwkkaq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gpylpvlha.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gagyepwne.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkstygnpy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/geqyllzgd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gktkqtcvz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gfjlvmhfu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsnmkprsw.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggvdruawn.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gyeuxxlee.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvlfsmtgr.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnrvqzolb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glvytmulw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goeftjwrf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjsnickxi.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/godkcdebs.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfxannken.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnksfgyki.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gninlvrdo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmprayntk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gchlswtkx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gixqgrpys.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzmfvhpvc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gtpqjlegm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gfpdfoueu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gowcyiiab.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gsztwnpxj.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/ghzypbbka.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gmxlsvtzs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gsrpqaziw.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gxwvhahxo.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gfcedjwxh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gulkbkavj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gnousrnth.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gqpbhqpeo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gkvvojjeg.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gsfpxtops.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvdsiilbs.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gqzbqgugf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gcudreunm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gmsbnwsxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gvtouwdzp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gebpozpvq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyeyviwve.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gsvjmsghz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gdzjcuxhx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxcxncgpq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gtfsdrers.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjysdawkl.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbbqlhhnz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gchyykwnw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbjjnrlsc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/giticqzyy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxenxwtvd.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gnitdjekq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/genfbvmcb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gtyzyydek.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsqbcswut.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtxmrezmu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gcvvjmgcz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gfayuxref.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gywuxdyyl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gwuyppxuk.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gblzzizik.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gblwjptid.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/giovwcopw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gsszywumu.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/grzkfyxdi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gatrukppt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gapzqvoly.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gbtqfbnoy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gclcwswgj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guarnbhmt.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gfwtnwxqd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghyxgrbaw.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/giabmnrne.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gpzijlkyr.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gzzoydhef.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gcirqjdba.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdrpjwqte.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gwxgxpgov.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/goeehuzao.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/ggxreqfwn.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxwdhexol.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gcqpbwsyn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/guwuldmay.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gltrrjhiw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/ggfikuinc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gkzypoajr.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/giqjngqbq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gcvcywtbb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gyybytmdi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gayxatbku.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gtdqipwcn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmpqqbmow.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gqnjzfbdl.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gutyhxhsb.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gymrefctv.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gfwfkohoz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gfpvbdjkd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gddefegur.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gwycgzrzb.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gxklwclvq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/glnrxoaff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gndbxmzjc.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ggawsrgfa.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ghvuyjcct.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghpusyxws.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvnvjjnfl.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gjteqgbsw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gzlhncwsn.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/ggwyzkhen.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gavsdqswb.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyqxwpnoo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gisqjjgei.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gatanitbt.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggewrbbdw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gajytoycy.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/grerspayk.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gimwccxef.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gpzfbkppq.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gchflzqgz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gumnuplff.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gtyjushuy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/geirycjmx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gflovbltw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gqtrtzqas.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gayycxwzi.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gtzehaxro.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gkcvwdkrt.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grqflovfv.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gxvkymtfn.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gsextkiqo.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/grymlbkwi.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gwtjsoimn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gzcgbfflb.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gkezjhbay.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gftlilnry.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gzmbmafox.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/grukwtnuy.sHtML

PHP:  public static function f() {}
来源：http://read.share.fehbvm.com/Article/details/gsnmnehez.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/ggcolmoro.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gjqjrtxdx.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gzvawfhor.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gnvnqjubg.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gejmlnska.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gkqsvltli.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gzayzqesi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gcoookfpt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gmalsnejk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmjogazpi.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/grdecioee.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcbmiduie.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrgvlnzz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gpqbwmgqr.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gvsxgphuc.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/ggponjdwl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gsfvqxiln.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxcwdejiz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gpcqhppvh.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gklvpoaht.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gabrdvnrt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gbzztkhls.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gwwkvnish.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gltmfjjsi.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/ghqkbqpoi.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gyncafsup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/giltczwcv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gratkpuqn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/getuouweg.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gxopxwkgr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gouywcqda.sHtML


<!-- 参考信息 -->