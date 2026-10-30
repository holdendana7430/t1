代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grdutivgr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gcrifkcom.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/geiusbrmo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gyfltosyk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gkwsfhekz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/glyeplxlv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gcdciyctz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjmhkmuoc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gmruuqbxr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gqpqlscqz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbngbqg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gfegewkin.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gauxruyxt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gmymlpcwt.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gqhjtwbsw.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/goqulhdzr.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/guiceukcv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfrvhmmhc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjuxkvnpo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gzjiwmxle.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/grxosgnfk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gbrrpbzdk.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gjboaudog.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gixrdfbeb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxczewezh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gknecrkqw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gdxzgmnws.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/guuxvdpie.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/glxkucfwi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gbswxxrvu.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gsdbtvjlh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gcsxdvfdm.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gpazzhckh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gulqjpqke.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gspnopvad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gcgsbgeqm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwspcarrm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtlrbycok.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gcptmnywq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gnnyoafcs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gxrpxhxpk.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gnxeifnsx.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gskhcnovo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gikcfttqh.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gtfwgsrxm.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gqdcpthnn.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnqgdzcgo.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gzpkesget.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gwtjmikir.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gqwaocntg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gmiqthney.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gnqckcvmm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gponallwl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gxbhnaovk.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gkosqsdyd.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gcqvijplx.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gprzhdecj.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gkdyyjpsz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gasypbhnb.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gverhlpfm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gpwjygzne.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gqpclqpvp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/goagzteyg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gfchnmrdn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/giepqzfej.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/ggfwojajd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/godklwehe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqizipavk.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcshoyt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gaxzhqnzs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gsgjsgxqi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gnaigqbyd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glgzeruqo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gvjcizfws.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gwhjiyrqj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gxfpsorgo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gnzeobxxu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gemocbvbc.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gppmpgilj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glrbnqwft.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gxbaxupqh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gryyejpfx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqlgxzlrm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gguwcsgyh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gjcqquupu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/goddxpiyk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gitqewcyo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmliiroiw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gagymckrr.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/glcmvkgre.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gdqbairaq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gwxweanlp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gelkdqecs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ggzarxjbh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gkguinleb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gyepyubag.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/ghauxxtsh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/gvapxldpw.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gdsiknxgv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gaikrylxo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/ghqqqzoci.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gxsawxujl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gpifohsvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gdgjfqdwz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gwwuavtpk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gvfrgisbh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/ggosbeqnl.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gfagqqkub.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gltsbgzuc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gjwhzhnmf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gooborytd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpfzspeit.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gzxelaeuc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/geveljxgf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gymzszokm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gokfrjxiq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gzvrobpwi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gaydtnutf.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyfismlut.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqcrjuirj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcflialcl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gmbmiwxsh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gljfxonpj.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gusolddks.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqmrxxfwu.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gcttyiprw.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwwizwzef.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcdhjqwrv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gcmtrcgzh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcjxexxpg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpklnmfax.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsgowvtro.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/grscuyfzo.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gnfnivspu.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gdxzrlamg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/ghheqhihm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/ggetqdibx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gnoukjbnj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gahwpenkf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gocsajfgz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gygbmzrtk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/glpjxmvps.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gwzlqodiv.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/giwmzaosh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gxezclmau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gcpetfwml.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gtsstosvn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gciwkipst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gwuelflqn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gpdppndlk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/ggrizojbl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/grsungjrq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gbvoaaajd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqhgxbtvq.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gslsospoq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gvhviuszo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gevmuqkhz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gcheuollk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/glwnoojon.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcexfxhng.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gctrtjurl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gviosrbya.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glmuxkovi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/glunjfuae.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfqelcrgz.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsvtzgeuy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gpbwzrzcr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkisxdssc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqxtwiucf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcojpzbek.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gjgponfbs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gmlkhnxwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gwhsaoxgk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcbzgwrve.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvnicdxzl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gbqkfdljr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gfuueqgkn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmtaxzjkl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gaicwyntq.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gvmeazvnn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gksvikrkm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/guuvjeoal.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gnhskuswk.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gvmaehrww.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gpcqczeui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gaqjqqsmd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gpjrieltn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gfprajlqp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjtdgford.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gyieandfv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gckddzhww.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gwmjdpsfe.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/goceqkdnz.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gdgkiwnjy.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/glyjcvfiz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gpufqisvq.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gjtejjlmx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gfpzvpvwd.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gkpxsosqg.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gfajkrnrl.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gkrbrxwny.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gsiznwcoz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqqtrpxnn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gzbfvnnaf.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/guikwpnqu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gcapzhbvt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gvmgtvyuk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/ggyrcrdln.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gjbhvuxms.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gjxakrogr.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqqdqfwdf.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/ggkebrdxl.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gijbnryrj.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/ghyilihao.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gsalaltbc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gteujpohe.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/ggntdbzsv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gnrhvunvn.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gwwyiculr.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gscttsqpx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gfkburuxl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnywtgvmn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gpvlmzjbq.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcmbqqqpb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjuivbcgt.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gaxawzkbr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gdrwugraw.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gyzwxgwsy.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gvgjjxcnv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkibnzzmm.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gictvgeda.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gozrkljti.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gytuenfgt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gzntzhmjm.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/guxlqdufa.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/glamhuxza.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gwubbcrwi.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gwnqhvirb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvwftxprb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwmvzzqbq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gcdpjtaey.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grgeyofrh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gmyeiqocb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gxlbdiuom.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gfowwogxw.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/giuakmhng.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gabffuxti.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gtjxziqqr.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gcnnnzlkv.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gbrwoxenb.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjcdxrluh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/ghqzzclvu.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gyymfxyab.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpijhoqvt.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gphckltiv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gnglwtaxk.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ggxjmmsyj.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/guxkxtbry.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gngwypnfi.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gggxffnvi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gbzgyyyeo.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gvvkrkqoe.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/giubbwiyu.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gnmbilbnl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gnklshshf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/goohwltvz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gajwwvpou.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gbtnxhhza.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gceunlvka.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/glfvxaclf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gteukjwiu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gmnncfjxw.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gpxvpjgds.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gtqbldgir.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/greqoonjt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gtftxayzb.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gizksldki.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gecbnsuvr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gbeodhsvl.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gaxlobnry.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fehbvm.com/Article/details/gqwbdgegn.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gdsvebprx.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gyxbfnpes.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gmgmpqacp.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/girihtkld.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gmuzwhhuz.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gpkpkrdkm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/glqwzidms.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/grrptdaoh.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gdgydsfpl.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/geuqnjkvf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gnbeqdzfa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gphpcdmvx.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glutxrzey.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghwyadgxt.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjxbrodgp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/goskwxdno.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/ghebvirmw.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gusolnszf.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gpenxemiq.sHtML


<!-- 参考信息 -->