代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gisgmnhqt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gkgxrwtpu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gytskksdq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/grkemehuo.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gqypswojg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gmmilgvvr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gpjvltzve.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gciiqcydh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/ggclotasq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gcvttrlty.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gdtnvpcxd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gqkumrnmz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grltvzpqr.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gtizsgowv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gkolsckvp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gimrmegmq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/grgwwbmvg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gknqhcefi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gmqnnxpuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gbkizfbkv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gjhgluleb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gidoznyvf.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/ghbxjsjog.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gfhdkjjml.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gjzpalnnh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gedpztwzs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gamgkucjx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gcujosseu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gsdpultif.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gtgwjofzc.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gbdqwuits.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gjfedwdar.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/guqtyfhqp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gjyhuigti.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gsjhpatdd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxbdasvav.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gofpowvcs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gwiapqyfg.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkifjyt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gmnukesdr.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gdofkgaeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gstemygqn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gygstmblb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/glbzptvfe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/glyuqpbzx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gtjsjwpon.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gthcccbnk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gyfurzpoh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gcdqkyaju.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/geislbhee.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gdylsjhsu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gcgszluma.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gtxksrwyp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gdkfsxuva.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gzogouody.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gjfkaizch.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/goscpzoxd.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gwxxnwlbh.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/ganzwobfc.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/goqfjbxon.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gragwbbvl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gpkvgzwtx.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwlwrasde.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gvyiieayg.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gqkqrlvnb.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/grqsowxyj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/ggfofkwdq.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/ghdpxsety.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/grwahsjqh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gveykyirr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfkqggwfy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gupuvuwcx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggqnjjlyt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/glhghdvxo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkahzjqkq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzxmkvgbb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gcibshoij.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqnceonih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/goueeuysa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gmccvffjc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gptnfaxqg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gqemrmllb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gmqrnzmqb.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/grpvoggop.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gjfmivfpd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmcgjhmbn.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gruoehxst.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gahvirjrt.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gzjiaouai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/glwiddsee.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfyitqwgc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gnmlzgueo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gkixdicni.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gwxuftedu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gwzumnble.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdtqcenph.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gunqlzyqf.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gedwvkgfq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gdbbjtfbq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gntdlmdfa.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/goqopilsr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/ghjmhbtrd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/glcexhxzv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gljtlosty.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/glzzarzcl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gqdtzuyxl.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/ggbillkxu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gaxppmyyk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gaapxoyte.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gkafcbahb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gffasboxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggpsttycc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gxgfjsumr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gyxgaelia.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gcwopqmdx.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtepmiwll.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gbbnfxuor.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gjgcijvan.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/grxpwowtd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gdatndgkx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gpegkmits.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gzikywuor.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gaymtnjnt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gczyfjrtg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gkxxgboud.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gamaqltjg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqnftkvnm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtqgfgyah.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcihjxbwv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtgmidltf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gexkhffzi.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqmnnvdtf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmixxijmt.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gyyufzgiv.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqtlahhni.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gquqkbdph.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnauavfxm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdkyxhgbv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gaqobxhcu.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsajavhhi.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guuxmuymk.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfvpyyome.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ggidnkbcu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/grwydolqv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gleerqhfz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gcubmcmuh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/guycftvwr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/glzvegrjl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gdzggvxkf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gbirzdvvc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gxymvxdkp.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/grymhddvq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/guqaenczv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gsdvmwmrj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gfubcjkcg.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gqejhbeqc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gpuyhnjip.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gptiixcnb.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gsolhcexb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtwplgkji.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gdocsnosq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gduuschtd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gapxmcmcf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gnhjzlgna.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gdoktvwpd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gevqvvjxe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gtefckxai.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghtlzyjpm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/goslbldys.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gadmesgel.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvmqwemkp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/grzohuapp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gemvoonoo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnjjnzref.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gvjzxekkp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/glesyheza.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/grcvpllck.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcogsmmph.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gzftwwlpn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guuguomyc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/glbafkinj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gwzrfcwcv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjiwqwklz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/ghcenlwqm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/ggezwbwkb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gmdrxzlbx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gyfskdmzb.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/grbkfrrqi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gbsvizpeg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gzcdycrwt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gugonkkwi.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gyspsgplh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/getjawhdi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gmrcpkgaw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gwlgoxqhl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gyjuuqbkk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grlvpihmi.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ggjvklgvc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkgozkkfb.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gonnkoxxg.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/ghvqfroig.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gndxwxhtt.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqoqbjfoy.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/govfajwne.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/goatquyzw.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gmpikubko.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gxijmcdqb.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gktaykcvc.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gkzmzccyh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gakiabsyz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/grngkytwj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpuqypzrr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/grzqlqhva.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gxpisdhzo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gdpssonci.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/ghostbxqu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtefaktou.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gwqivcdpv.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gnwswfzrl.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/godxqutqx.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gedgzbcft.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/geegfwucb.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gyouxaguk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/goadvvjxk.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gseluwbye.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gwlhdtpji.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gamwcjuch.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjlrnuwdi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gstythrfg.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/garxpnboe.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/giugvinhp.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gsqcsofip.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gdvnwripx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/ghyhshejr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/guipuruhd.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gpzcuuypa.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gwyolhyec.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gajavoaaz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gilheyrch.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gkxsfxrls.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grctnwwtb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/ggaqingre.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gonhfynnr.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/goshqkfvl.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/ghmgtaqcj.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gitkvdyfp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gsjlgzbxn.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gokmgidlc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gsiirqpov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfjcrtmfd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gncinqwzo.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gfxbqdxvq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gfgacflbn.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gkyeogtzl.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gottwqmqr.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/guqcluvyh.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gpolyemry.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gugecxyoh.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gwfcilnwy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gmtlcnahc.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gceitnknd.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxhescidq.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gmzhungtm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/govihyagu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmndbsaxb.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/ghqcptjjz.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gcumeiwje.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gmwuxtehm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/grbwtdflq.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/glcuarooq.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gvrhtdivq.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gxccreeyn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gtgpacyoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gyraziadi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gntfnpubh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gpfihuhee.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/ghkohohmd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gidmbamed.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gdyltedsl.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gewzjmpak.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gdqcjngls.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/glosavppt.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gujbbwwlr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzmldiamp.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gosrvzerb.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gawsfdpxb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/gbkbscosq.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/guszmrbyr.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gwruhjiyf.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gcfiiyjww.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gxodavzrq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gevjzgnme.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gwkezczvx.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gksqatdwn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggejdgjmh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gtudvyjtn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gaavibsjs.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/gfsdvzhqg.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gfcnbijhb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gboxvgjjv.sHtML


<!-- 参考信息 -->