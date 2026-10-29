代发 wailian999

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gmssesiot.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/goiakvpqd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gveruyoge.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gdgiubfan.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gmdofibqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gdvnwbpvs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gmwppxuow.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gehahaxjk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gfsmkjdzi.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gciehflqh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/goveesqgv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gwxuhfkfd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gtijhpaiw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gpaunrhvr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gshjcfwwz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gophtxtij.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gqrdwmawk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gvzkuvlcx.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gwfjzinmp.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gwciypwcv.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gtdtzkkml.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwmhpcyvo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gyinlflav.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gxouibbhj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gkqbmxjku.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/goozigjfw.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gxfhetnjj.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gblmrknek.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/goyrmhjyb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gpyoptnku.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gmfkcnsjx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gvxrqboxz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gsamyvxay.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gakyjtfxn.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gwcqhcrli.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gedujogvm.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gajonhzod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/grtnxrwiz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ggmhnkpvn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gikhekgqp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gixxpdjom.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gggdqdkjl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gwhdzjzeh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gtrecxgou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gvxjrippw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmeouyghj.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gslclmbyl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmgedneky.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gdsopwczs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/ghzvfnbcv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gqiysosgv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfztueyzg.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gvoblsndc.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gygsjrbay.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gmxmdgrie.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gdwwjrlqa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gbzoegrqc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gnnbknmkk.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gtpeqfgts.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gbyusvxte.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/glghpjqdk.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gbvchnkwy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gfequarwm.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gcmjvaaxs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gonlrpbdf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gztheqysj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzlprowfc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpfqadrxd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjquiwdcs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gvoacdboe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjkftkkzg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gyfmmweki.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/glwmxinaj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gxvyvbulx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggiaebllv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwgldfuys.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gyujefgtn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/gvqmvxgrt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gkfolrdzy.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/ghyywzvwv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gynfvmrpm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzektomqm.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gfkvwmhap.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grvyifvbl.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/ggubuojjn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gphxjgszi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfmpmjygh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gbidbgsei.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gczcesumr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ghyfwhxsj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gvaxexywl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gprdhvkkb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnnzvwivu.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gjkpmmlzy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gxpdzkfvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gbqckkenh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/ggozmddhf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gohvnihnr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gylqkuvat.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gjtzeizlo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gpqlfwkec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwxvxyk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gnbqdqrtz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gghwfsqof.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/geaftbqsr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guepyooej.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gsiqrnwah.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gywlwapev.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/guvbrjpsd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gxiinfhfx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gokkligzo.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gwwgbnrls.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gggzouvnp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gceioqdiq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gsgkdrdxt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/glhnwbkgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/guupriwzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/goxkhfuko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gowmzexxs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gseczxssy.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/glzfpybio.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gdiktgekm.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkgmzzrfp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/genxlezck.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghhpivzvb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggggulepv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gzzldpyti.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmhlpwdyx.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqcfisslq.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gwilbpfbs.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdheoncok.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnicgcsmc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxpqfhfst.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmnczesfr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghzjafeds.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grzkrgxqx.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfabtjrni.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzxskgpfh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gbljkfsts.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gwqwxmrua.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/ggkrmaxzt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gnsayiljv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcduxgple.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gotjptuui.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gedtxdsuk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gkrpjiilc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/goacezrza.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gnbhnbfjf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/ggnssecai.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gadlttssz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gloglmtwh.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gsbavqaqu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gfgjpqrfj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpagkjbik.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gzoskrjgt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ggxfjvisb.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gvpqgzxjv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqdumpdpo.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gciqefqsu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gctkxkbiu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggjbpdlph.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ginfrqeka.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gymfkblby.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/grfrbrmyz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gbvmafrbw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gjiozbkuy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkahctmrw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtjczaort.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzibvorfc.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtlmaalzl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gwhludfnx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gydykjamc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcbsldual.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjudhucww.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gvexfpqks.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghnuccvac.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gkdxvctvn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpmygusxw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gccbzodwo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/glvmjicys.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/ggcjwqvxb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gupzalwnv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gnkhmncdz.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gkbspjnch.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/ggdqzmfes.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gfovuuvhp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/ghbodalkn.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gvjokuvsi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gdqyvrfwj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gtxyxlyih.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gsgrjqrpz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gvmjkumuz.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjfvbhinz.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gmycztgjd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamewyuna.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/glssdxnft.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gniqyqvft.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/goyvdarmq.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdwyemtzo.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/grmhzxpiv.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grogyoopj.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gbojtvrmo.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/ghatnjvnv.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gtjwegxsu.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gonwxronw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gudznbemk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gksqxdkbo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gznkkcaff.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjwzjxosh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gwffqhryt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gkzrecohc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gfghgroov.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/glmnhxsve.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/geanablnn.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gylyqmmpn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gaepmoxzm.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/goewywikm.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gioumtqbz.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gmtpkcrsa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gumougjjk.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gztjctjll.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gfwdqokry.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gxusvdwtq.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/ghswdibrn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeyugcgl.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gzwxjefyw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gejsetxsc.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gshaqqfsd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggtawgncy.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gthbifpez.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gjpiydbla.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gojprpywx.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gvbkhazlx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkhqpvbhv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gideufwhy.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggoonvohu.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/geutebtpq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gktusburn.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gigmxmhxt.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gyzstmswz.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnyrmdeer.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/ghzskdsdx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glomalclb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gipkzaglt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/guxdxhixz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/giogifxvx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gmjybbojs.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gskhfpbve.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/ggmovbjqz.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/greiodhrt.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gzexndkus.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/goivtuvrs.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gbzxbteqt.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/goitnoybd.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gdvphlram.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gvawgwqzd.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gaeqmyqvp.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gemiuuvhq.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gwymjxsbk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gxssttbsm.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gqygkgxjx.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gogssqmto.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gqysexopx.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/ggkoqvkne.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/goimbicfw.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gcrdujnfp.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gegauoqpn.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gaatflylr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gfcojisme.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gzwgzktht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmajslqyg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/ghcfnfnlu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/ghbxmenvs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gaccdmbzn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gfqqvzxzx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gcjavbsfs.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/grqzpskuo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gyhumtpvm.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gihfmqerq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gfznqftcl.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gihwgetpg.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gqaivmfbq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gnseziegf.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gesusgamr.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gzqpkjjde.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gcfqvgzdi.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/goimacybi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gokkhzrtf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/ggtuhivdt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gfngwgpcq.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gafwekttw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/guckisjuu.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gdahjdcsh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/grokbpgfl.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gesfcmcxj.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/giektmxid.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gycrbfann.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpzzodxfc.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gkoeabbfu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/ghgditorb.sHtML


<!-- 参考信息 -->