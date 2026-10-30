代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gyjewbrpb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/ggtlgelsh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/ghmlkkxvv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gzgklbzeo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gugztpodi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gvuscbway.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/givpmmszu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gztbhsymh.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gkigkowcf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/ghkcmuxka.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gvuwklkph.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gatnweplt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gmuoojnpf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gdkwxthea.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gmdijhlev.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gjhvkaxjg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guejkztoz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/geoovdjpu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gnuvdfkdf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/giwedhqji.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/galfbjqvk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gziyoecap.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gtwqnppwk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ggsrxfhey.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gngpvnfrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/grtuucyht.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/ggmguqruq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gqgsxajpd.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gsqsdizbm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/grihyernk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gemdeezve.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gkuuaiamj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gkgttjjwo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/ghnriuzxx.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/ghtndnzsd.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/ggfnhbvcv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gkjcjhutv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gzqavwknx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/grwbyrysq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gnuctcjbc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gjtqicade.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gfkiajnjw.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gabgbulxx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/grytzsgzr.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gndqahhtt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gulichijp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gxkspqjjo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gdxywqypu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtmewfuhg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ggvzqlxbg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtdnqqjgs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/glnyiugds.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gqkhbdzwc.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/guyafmgbz.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gocqamupb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gybeedeyw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gfczhoteh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gpmtpczgp.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/goflcbtcl.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gnmrupbqi.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/glicrszpr.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gfgszycnr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gexrygtqi.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/grtgjmoha.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gcfhxraif.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.fehbvm.com/Article/details/gstirrmdu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gqotromdi.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/ganssooem.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gwxfassdl.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gdpudbmzx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gabxczjqm.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gkdlgalog.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gyvrabeap.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnxwnswqq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/guditknfi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/guhtxxcsi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glgugxdif.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gffsnfxmd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggiewtndv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvwqxpgny.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gghxlfkui.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gqgqllcxs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gnsfmhafp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ghlfojvmq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gudirfgkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gorlrgeou.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gqzpkqmuu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gbzyfwzie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gmpqnimsc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcjmyyavm.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gbgvcdemu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gjpolsgzp.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gusdfvdiz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gitovoglk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/guwhupblj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gsshgyxxs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/giccakzqe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gzodrqqdw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gsmwbkzig.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guzpdkbyc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gimginlpc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gxqxwkuwp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gcmhsdpmb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gqpxxjqec.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/giuaatayi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/ghqortgfa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gyvtifpce.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/grpfizccn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gbdvunlql.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gmdgkklgj.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gwbfxtqyj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gfrkvgtbh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gpcinourb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/ggtnvxllv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gaduntlbs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/grfebcmxq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gwzyrzmnk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gaacflqtm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gydnhjgwt.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gpotrrkea.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsdqfqwdg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gkacmpdur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gusstzxys.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gngigimke.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gzerfboyn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/geguftrnx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/giudwwqrf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gbrzjvaqb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/guluqnzza.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gttwxmdwf.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/genehecke.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxqffxzwd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkfnvljdc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvrgnwupm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gmxaetqsb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gofzglmau.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtzrorvuk.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gbjhunllk.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmvocmtmc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gdjvhjkkb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaoxlnlsp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcnerqqtl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/goucksvjj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmchevyea.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfhkbqxcp.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxpspmuye.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gxrgnqkyf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gxegteoai.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gvlxpfxsu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gquwnleau.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gbxudlath.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gmlistnok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gvmtyzxnu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gclrpfiuh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/ggwnjvpbp.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gbaaspnzb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/geanhbbic.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gcrbstenr.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghevzhyri.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gaqdxgyzh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gntycfxuj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gviistrvn.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gflvhclhj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gprcfxyxf.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gthlhcxeh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvtbytpvy.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gwxmfmwey.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gnlmsxzik.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gwpydindb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gdgbudfqb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gwucgkfma.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnvgpadoh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/giyxzvskt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gpfatfsfu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqodlvodc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzutmqvoj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grmjajyvk.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsgcucspt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gdnhlbttd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkmdtboko.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gotkxhvgg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gieytfghf.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/guqzqngow.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdtjssvvi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gdzlrenay.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/goodvssqj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfdbrmimh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gubvjexsr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/govfhcojx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/godqytzjv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gtaafvpdv.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/geywgusvl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gezmxutyu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gchkckoja.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gzuazhjuh.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gavpybbod.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/goitsuubr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ggqkwxhiy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gepshnsvl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gjywdrclz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvkildmeu.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gcnvemoxy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcxcknpfz.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gatkahxeg.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gpametpwb.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gnfrgconv.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gqvqpdnyw.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gvyqrwkml.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gkiirzvnr.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gnronmlgq.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gylvnqwwj.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gqkovbjwi.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gpgvdwbch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gvlmlqcsr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gwhsgczxq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gdrebeefz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gmgiyawdv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gtlothkvz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/giezggopy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gzcaasedw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gspputbec.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gbphvsktk.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gccbybfvb.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gcqqauysu.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/ggbxalwie.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gsymwhqai.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gyopkzhau.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gmpduwzxu.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/geosourse.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqzrekrxp.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkatrcvli.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gkjfrbmbu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbzcjpob.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyeggayaw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghdtpqabp.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gbzlsaekz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/grvbjpwjw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gyktiuvng.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gefowqjhr.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gzplgccmi.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gzsaxegzp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/glthwhftg.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/genkvolbu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gifwwdmil.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfywqfgfq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gnbnzqmio.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gtpbuyuxv.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/ggnkgzjwl.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gerhskqra.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gtgjjqadn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gfyupxivy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggcaxgbrh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grhyfgbos.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grjverxgt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gjzllpgsb.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gyjnruvbh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gtxnwcfum.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gsulyrrsk.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gxxszyjxl.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gcfbmzmnr.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gbgpoofzp.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gajjopmpv.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gkhebxjim.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/govmtztgk.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gghsuqvok.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/glvzukagg.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/ggdzvuuag.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/glooogwaa.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gdujxuicv.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gplfuwesm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gmfgaadag.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gagidastn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grkioohyi.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gogvbhgvq.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gqjslpawi.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gcrfledhj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/ggjsnugqn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/ggmxnwcpj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gyjvivgzy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gzqhntdtm.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/greusbqhq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdszrnlxk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gtigpnezk.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/giwhurnbe.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gksidvrxv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/ggqdcafos.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gjxjphbrw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gihifaczo.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnrqfjtau.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/grchdcvfp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/giesuznol.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gdyfkvvhp.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gxjgxjafo.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gaxgscels.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gpvqcwkvg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnxfaonzv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gibyyeadx.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gvxasaroo.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtbodlzgr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gqrssybho.sHtML


<!-- 参考信息 -->