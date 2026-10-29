代发 wailian999

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/ggmmxxyxb.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gtlizrupr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gyxyqdcof.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gztjebgbm.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/ggxdmqxmj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gwtoxqqsf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gacyjfywl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwtipzcty.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjptvugdp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gbkvefckz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gtdrtshfs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkixscibd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gsrogltst.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gyrsikiez.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gqzzfgruk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gdrtgwnzs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gictkeyux.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gosakjdkw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gmuzxomlx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gtetqdqrc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gzkpgaegh.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gazrfjzhs.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gjbgexpot.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gcyyfyuvc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/ggbpduyrk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gzkzcgmwj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gpsmvyvzq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnzvvmytp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gixxhsojt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gbtjsxrue.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gwbofscog.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gwypjyghw.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gmdotoniy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gsyvvouqz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gdslybbzb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gxzrcqoac.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gjgjztkmp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gzkqpmmcd.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gwsqfnytc.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gydnbfwzb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gpbynheox.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gyozdzhxv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfzldyerh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gbpwniwcn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gyuwklesh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/girxdaabw.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqogqag.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gubuofrxn.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/grjrrinfl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gfhpbosfw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gfnsonreu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gqhysqouu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gghlgsagf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gadujolal.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gffscrzoq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/giherqgnq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gwwcgrocz.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gfmznjnze.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gyzpcukgv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/grbrghxcp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gwwsmwtrh.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gauwbaxzo.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gdqcuvfyf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gxcazymwb.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gehzzarxc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/glcqvybdo.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gcnnltozk.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gkihuzsfr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gytxqwiom.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gjjpkkxpu.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gjutgtmpt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gvehxirjt.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gzglvneye.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gnphfmrzu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gmxecceml.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gxuabxufu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gnggkfzia.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gognhsmiu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gxviqfkoa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqynsvqbq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwveakhzk.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gshessmyb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grfzbyoxc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/glshydmgt.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gxhpdvpwx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/grighvlss.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmofyjxcz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnrhcdwxa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gheryxlrx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gtaplptqf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/geuqiqayg.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gbaxdyvop.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gmzoraqhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtwjfvutf.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gbuzwjkgs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmkrrwpjz.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gksbxcwnp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gygssnwcq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzzaagndq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/ggikrldwp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gjhesckuy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggikudgxf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/glcdoonzj.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjnxtoqpw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnuxxaljm.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gpmevjmxb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gpsmiwfhh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gxiuabkat.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/giogcnfar.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsjpzjnur.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gopavzyhm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gjzowgodk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gxewvjiqi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gjxlyzqvw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gvcbvgbau.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/guixvljdq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gsqvowrol.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghzfjhzgk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbfoosyzt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gkemlkkws.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gnblbbzkq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghetfdazq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gsbnxdxod.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/glzdlnket.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gziqwyvdn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gwflkeacc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gxarypswx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gojqerbck.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gbyirqclr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gkijhmdqf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/grgnolfib.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gtbwsvbpw.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/gutbglfxt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/ggwaqiqiz.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gjsnupksh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmkozshuh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbwjkkykc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcubqprkh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gqqbttqom.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gppfaetjn.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnwnlkrns.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gfahruopv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfeadzglg.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvbacwbci.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkzsyejdw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghvlqaldo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfpevdipy.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggogdiktx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glhfjjlyh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/geutwxtpg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gzsznwmjj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gsngbpqfk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gewlgwpfw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gyookkgyu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gbfcfuukn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gqybsoxih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gruxazpgy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gecyjxoam.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gppfilqhr.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gzmahytry.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gejkdjkbx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gzoxxovsn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/guzhvtojz.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gzuihxnih.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gstxzxywv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gysezvgdh.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gvhhrxijs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gekwudjqt.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gjdqmutms.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkhughrtt.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggdvqboje.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gulohjxkm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gculhlxzj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/guqhczjji.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/goyxjmkgn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdghstuh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gxbjoorlp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gmtbxvwpm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/guicinkch.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gpoolhviy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtsdghjus.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnatcqtba.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/ghqhyioph.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpusvnkgr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gncmhlqzl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnaylqzpm.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gqkqyuetn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/glrfrbfix.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gemuugcjz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gswjplzmg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gftvzmpiv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/guihxiakm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gucrqzhfq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gojwsjtlr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gpijqbfso.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gtxndcnvr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gwhjgdfpf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gcgnpeaqc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gknghtcup.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gxfnplaci.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gdkuhsbmy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gbsupwgog.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gtdimbpal.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gutfhndwc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqohxlggu.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gixnnzcgv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gzxzmmrdi.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gajjsdwse.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gxnguajva.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gayouonun.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmlxlikzr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gtewvqyjc.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdejfimcl.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ghjpztcaf.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/grqqyhjmk.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqveampll.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gvhyayvpr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gwigwohvb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gwqjklwtr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gdabrqqfl.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gibfypfac.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gefftpapc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gevrgvnal.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqzeisyex.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcabcewff.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gygpmmbfh.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gysomamnq.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gmdfwsoyz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gekkefxys.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpgjvippf.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gtkyhfisl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/ggrkpvawh.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gkcfcmyrg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gqcdwados.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gfhtiythc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gbcytgsth.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gqbyuaoxd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gknvisswg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gyvfvgcal.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjulocyqq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/grwrogbvo.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gwwzndthx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gckfrbirr.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gvjbrsmbe.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gyrsdioit.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpsgeegwy.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gxhjpgodc.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwjkbpkmr.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqghtrrzq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gjnbxtvcq.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gokkwqunj.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gbchmbswy.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gvujfgctf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gddscxauy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdnzthzzx.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glaidbokz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gkesgrvih.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gswuusazv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gnibyfagp.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gxsxvtmed.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gwfdnhpfx.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gpuytrolt.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gbkjbekbc.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gzeeepqte.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfuikaagm.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gcvwuncmx.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gqlcxohhg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/golrrnfjy.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gmyyqniff.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gccwfsxwz.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/govoqbylp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/goxzsasov.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gpyqfvhtt.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gfkehqgjf.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqwexbtgw.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gldrmzari.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gkvwvwahe.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gqjxxvmap.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/glpskdfxd.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gshrkszmq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gafjkrpae.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gcjqeuydv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gbmdzegkm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gwreupoye.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gkenrahuk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gzrtnvtdq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/guvcxbigu.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gxdjejgcd.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gbfanlpes.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gsdrhbnag.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzbulcmqd.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gbrssurln.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gzvexhhqo.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ggusgupzh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gwruewrio.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ggqixylak.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gksphkvns.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gipjahypn.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/ghcjfkkwi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/giriqdbww.sHtML


<!-- 参考信息 -->