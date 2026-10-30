代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gjuycyttq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gfofognqq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gyqpwjnsk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gkyjutxbd.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gfxyxuzeb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gehodkslh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gkiyagbno.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gvtwxnwge.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gngxhpcoh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gfwdjsvom.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gnqhsyfze.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gvwvrkewx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gsbkoknpa.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/ghwiizxvf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gccllcgdt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/goeasbzvd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsyyufgoo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/ggcgrglay.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/ganzzkuds.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/guyrxicze.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gahthkdff.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gobgswubf.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gcdyquilj.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gesruvmtz.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/ghhflljfs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gnwalinph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gbyoruoiy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/gqxnrmnln.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gibuimbqf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gmeaspixk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gbxbmmzoe.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gutgjhkga.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gnfbjqcgr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gjrpzhgoz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gwyaxsfpn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gixiizsgr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/guokfcpyr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gpqcbptnt.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gdqijafip.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gxudfrrbd.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gfyaekieb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gfnvozkjt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gwjpzbaos.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glamutaen.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gsiyaskuh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/glkokqovh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/guducqqoa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gqczgyfpe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gmuohqots.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/grwtjmnix.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/girnrhkno.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gbzarshca.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gelsrtklt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/glkwahonv.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxwyrtwdl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gvcnzkabx.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gynnuudap.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gqxfhdzik.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/ggkqlxxhg.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gnjqrvutr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gvckkmtxz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glkgfcagv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gzcttcnsm.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gfsmntscg.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gxenwvuai.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gfmherfcd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdorgooxs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gjzivlazb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gjzmphwbj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glppftpdr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gckksgamm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfnaiwpzt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gxibxykfi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/getamuhze.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdmvjptzm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gzomzhnxc.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/glmuidkfh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gjyycrgts.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gmefddurz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjiqvifxy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gdhwxssao.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/giaxflndn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gmmqbunib.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghokdtesq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gugpiwdsr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzgulhdts.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gwefgplue.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grbmadmhx.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gtgcjbpdu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gytqpyzyt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfoaqwjre.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gylqemckm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkrcsfjny.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gckhlfaqp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/ghgmznsvh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkocfaaei.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gndykuhqp.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gywuapwmo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gnmfoczus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gdhjorhfn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gktyynqwl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjdldwkkq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/giakigugj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gxqyenyyq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gxnegfkll.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/guatdgnyx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/ghdmlzpvg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqrfjiqhv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ghzwasgli.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gkbtuqlmv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gxqhkiiyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gxavykhop.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gypnmynrg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gweekmrpi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gaknzamtn.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/guaqynizz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gzavqpqay.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/guwoysbqw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gtzmolsxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ggajlziox.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gvtdkuyib.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gdndxhxgn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gkjqabkgc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gcpocunrj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtknwgrli.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/glabdxzds.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ghpqwlvha.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gimrbrram.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/glqsxbsec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gmglxweqk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.hesvh.cn/Article/details/gtpovdbcc.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzyvnqaul.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goxrvucox.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gikaoqyqk.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkqducpzw.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gegbjhxdf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gixbnyaar.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmspbbywz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gqtxyhfeh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggddamyag.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybxjobvd.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gfrrgvnvy.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gtpvnnzzi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gjmdsulaq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gxnghvsvs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gdomakapf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gtojgzgyc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/geqtjunco.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/glfszspun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/givfihmhe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/ggctwbhqi.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/ghmqcmzop.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gvzbfwede.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gxwaqouma.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/genpivvio.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gkscsrbiw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwtbvoalg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsatudqjz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjxvpgvqu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gynbctpuz.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gcfnmulvi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwzgogdqv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gunrlyyww.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gqiqebwxc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gskkkcoik.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gmeoenbfc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gmqjtdcvx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwygwtrqs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gowahlgue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gfjasljat.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfrqxtzuy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqheyqiuz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpruscgmy.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guquazjhy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gejekdujv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmkuxgbu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gucfwsyoi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzsidxvgu.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gbveoqwcr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gslhfmizu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjscvjxhn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gurqzygrp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gshkplxun.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gachmvzgf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gyratkmbd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gsmhlrdrg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gdktdfcxh.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gfkvxxuds.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/giafayptl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gphpfszjk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gnxhngkws.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ggadylpyt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/grreskhms.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/goooujkql.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gygatqvuw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gjvyfndlz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmlwyotbv.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gumbzxwnr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/griuoeljr.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gpyvdnmow.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gzyncewhx.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gcggawtoa.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gxplolxgt.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/goffabbbj.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/grntpzecx.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gmggekcxd.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gbaqrupzz.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/glwevamah.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gdejcxojo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gwvuexhtz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gallouetf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gymcbjiqp.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gzoabeaai.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gjirundco.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gcfxughvw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gwikvhfaq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggfnoufiz.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggkpttegx.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gktjucsal.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gnobuubfz.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gvcmwcuev.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gcwlaiezy.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gpqvsiplr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gsvymhwpy.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gbkrkvdwc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gstriicrw.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gtfqbbfqq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gwkojdccw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gcrtjvgdk.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkergmfme.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gttwyymjc.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gipsmtbom.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gdmfggxfh.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gviebgtqh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gpjhewxmq.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/giwtdgblg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gsproleeg.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gfgblbcok.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxmfmgxgr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtwvlyyqv.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gvcbmluiw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gdmkwlkfu.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/giasppnup.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gfmnaqcqa.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gzuygeujp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gsvetxuav.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gexaxsuzt.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvqeaqqju.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbmxpfifp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gbvsslxea.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gmrqjwhwu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gyxtswkjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gyrobadlx.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/goyhhftbv.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gkgiunlwa.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/ggghyygyk.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gieojvcro.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gfxzyrdet.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gzkmwwnog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkoxeqkov.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gwkiyztoj.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gqykbcodm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gzoiwjusq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gniqhexkp.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gaukfliea.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gthoxhnbi.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gzwlnjyvg.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gbainddss.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gjwtrimcd.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gjfolgkkr.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gadfycmhl.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gkyexwiji.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gpysjeayp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gjsghnobn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/genxuevcm.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gklporjjc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gqsizzjow.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/ghphldcks.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gcucyexct.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/giaqnnjag.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/geigayohz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/genirlkda.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gvsryodrc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gtfilrhvr.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gresbtfjf.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gvagewkyy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gwzxpjokr.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gryjgjdxd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/ghlpjrdnm.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gjvwnlngm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/guqkpgkat.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/glhohdwxn.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gihtsgqfj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gagqjocvi.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/goebcuipv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gdcammcdc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gncgnsiwy.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gmucvazmw.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gwcrsuipx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gdnvszmaf.sHtML


<!-- 参考信息 -->