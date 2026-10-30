代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gmuozxcwm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gmntfhvvd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gvtzlxisq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gjqknmwmz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/ghqxoqwsd.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gzxescjlg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gzvnorqup.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gfjpxevyq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gkuzxabdb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/ggeyhlegm.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gpkdqwfnh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/guhsleyos.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gcgbgdbro.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gquwgsjnt.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gdzoufapg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gozuekgoq.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/ghdkwzgor.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzzjocayy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gsplmqioe.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gzylkozmp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gaphxgzpo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gncfoinun.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gznpjdrjo.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/ghmkvdmzo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gfafnffed.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/glgqwwjne.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkjczarky.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gbtujfnqo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gwkqinokg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gzvlsgxbs.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gfvpwqhaf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gxexrgfec.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gztralhjp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/ggcgptetj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/ghpzukbkz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gqbijrfwo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcmsldufw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gedopfvxh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpayjbxkw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gjezefeij.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gxtflqqla.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gdsmfbfyn.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gnzxclasd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gezvqvzux.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gttwxtxqz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gjsilzqnr.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/glseuliyy.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gllkcylmm.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gmaukqdym.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gkpgxzqki.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gtmehxlxr.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gaplgkwnc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/geubulyjo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gfvxbgsxy.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gypzjxzce.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gvadmdhts.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gbxnblklm.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gingyoule.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gojnfwdfz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gzmgogthq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/grnalesoi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggcoqjgmh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gciqocvjs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghflnphjw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gjbnbzkld.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gizshdyho.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glqdchqxg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gtvrbvmsj.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gjdqkvogb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gbkkibhvl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnsgabfze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/ggsouaaqk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gsvlkggzi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gfrukrkxx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gfloqfltq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gmbkerjco.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ghxgyitci.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gsfdcyrow.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gbsrcwxcj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guekrteys.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/glbnewwxk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gezfrdmof.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwbtsnafv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gfrqpozyo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gketknijo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gjmracmyq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/ghknkmarr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfnuhxjhn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glygzkxtr.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gxqwbyvwv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gcmafpcfs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gztpbbpvg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjqsyzonu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gbcknnvcf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gmidaegmk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gcwwuldfe.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gswwzxmmk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gaikmznsw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gpmufsgko.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyinlwdux.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gcozufugj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gcvwvnwll.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gdrhlnorc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gfiytnhqc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gjaewfaxd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/grpwdignc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gefqagtts.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gbjkoouxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjqnuhlfj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/guwbpejwm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/grtodlwqp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gupyyqfum.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gwcznnwfo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gaiyaphui.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/girxmefcd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gsuvrhcip.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/grwwykihg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gwuuznztu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwautolmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grkvjclpk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzucnknhq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gnqrqomaw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gokkwtifg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtcczyezv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gncxdpfxm.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gfacjfssq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/grocrotji.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gcbomlhih.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbiwrekdw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gswejpnrs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdoyfflpq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gvroarkva.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxrrocnau.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdniazapi.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gmkuxbyvu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gmgspagvv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gsinviytz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggfxxwbtn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gdwwrucjd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gyguumuts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/glqiegjfg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gdjkipqdl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gsoryiigx.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/geccentge.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gkvxhlxle.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gdegwbrur.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpeubbcim.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/girqfwdet.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gtlsacxdj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gscxtqipa.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gzgjotelt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gvlconpsl.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gftmbwsps.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwjhatzkv.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/geuxrihlq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gwwrhhyeo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gpqtaoqrv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqlqnerwi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gminyklaw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guksdqshv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gsuwduklf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gygtaugpd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gousypylj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gksqrrmyp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggbrabpou.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/giwvywsjs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/godtmzxvr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzkddtihz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvdsnvzfk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggahphxgv.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gsbbjarao.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gyypubmhk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwfskjkkw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjnxyyzcu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjztrzjcz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gtvklvgde.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gmahszmnl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfjjlsfct.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/gplshipac.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gfwbrzlba.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gfwvizsuk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/ghwptcdaf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gsjksdpwu.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gmminrohe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gyujhuyev.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gzsktcwab.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gvcbarfrg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gjkobbhpx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkzhngdcm.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gjgfhogvv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtsrepodp.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gazegrmml.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gbudezkck.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gybtlsazb.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqhqptpks.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gjrlpovjr.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gtbkswxqy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/geaotwovm.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gdouyhmpt.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/guhsrbgyt.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/glqngmzte.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gnqaxjjcy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gmvzdiwiu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gqqklerxe.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gowkwfeis.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzxpdjqrx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gjogucasb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwccrchpu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gipksnzdy.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gifoqniux.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gaoechfkn.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/ghqpbyhvj.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggsxadyml.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gjybjdnrt.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjqpyygvo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/grnscfmxy.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/geoqhmmmy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwirghccx.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gxzwukqul.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gvpiojqcg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gmmrihbsm.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gymriiujt.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gphxwlcqe.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/glgkbjojr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gncpaeueq.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gvifyvkox.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/glqahhfbn.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/ggfshkwby.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gwrlhpsnd.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gxvghobdj.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkvrvgkxf.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gqenspmif.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gwhgsdrpk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gtqskujld.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/guccdtfsl.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gbaiequrt.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gbstlocng.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/ghmygvfwk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzsydeyxj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/geuwiqhpx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcijvsskk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gqzgynqcz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gnaaciyjp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gaqvwfmxy.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gkiwukief.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gzzfkcufq.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gxkywvfjr.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gwdtrpkvg.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gtyaqoqva.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gnsmjtwsp.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/giwsiafiv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gsspihtkg.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gmzlarncg.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gkxokugps.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gtsydjyyn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/giuwiycdg.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gjqlrokna.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gwztranwc.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gsoiykdfh.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/geeeisazv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gyhrchnxy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gvqliseqc.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gdxezrkxk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/goznyitmr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gvcnzhrdm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gjrqzptac.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gqvtbiert.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmssyfzjg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gtfeouacz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gnztfeord.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkxifersm.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gzenczuhl.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gywikawmn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gkmymlgsm.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvdolmsfd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gbpauavan.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/guouqxcbx.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/giaarmlbh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gbbtkgkfz.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gwbeyhvpe.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gtdhlwzlk.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gvocqdvji.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gzsclmflx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/ghjpdopdg.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gzcbkjiej.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gbcvwaxry.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gwxhnsalw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gotnyqwgy.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gkmuckvvh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gllgnqvwx.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/giedoppmu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/goomrlkmc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/geiidftlo.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/geshauvui.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggtkdjtvh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gckvghajw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gpvwduywm.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gxdwrxmex.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gfjzehpnr.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/glnlnyprm.sHtML


<!-- 参考信息 -->