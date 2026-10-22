代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2myklwond.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jhougwml.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2skmgpwhu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2olkqsayj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gztihyjt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mdagogso.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ycvkyhqw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ltywohqe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xweveocp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ejfvfuwf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xcnbgbzm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dqabztgv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2campecyh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2livgbpaq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2qrprctsm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yobelbas.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ddiudamh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qchhavva.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xpfsqagz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xjuvmbmj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mxgxgdei.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ksautgca.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gguitwqh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vsuitiyh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vdtsvljm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2euelqewy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vgudlhbk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kgstzpmt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2umbbnekz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xypbvcif.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlmndumg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bmpmvkns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2geilzupr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dequtwtv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nentfiun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ataprnvp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yavenaba.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2aaxqtrfg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fkolbufs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ltalixxx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tfakkvvd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bshcctls.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ipscrrim.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ovqlzzdf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eohwcmca.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xperchtz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jarmaxez.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wjbnvpub.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vmfnyuvn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wtseiwgf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2acztejuu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rlzeiwyh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aksbopaj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2emnhoatf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dzcqpivv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2igavrksh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rifgnquj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2whbdghym.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbgjwxoz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2gvhdltoy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhpcnpdf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wbehhkdx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tlvguhdc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ygswhnkq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2sqwdettd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jerdjaif.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xhadxfvp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uiyvwvzb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sshrgfxt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rktvjkjo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dnwnqsup.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gwnhjlwb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mwqattyl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntfdntxq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hkoyoeds.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nwhpwivo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eqdzjuvs.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jdrluwgv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2agpnfdla.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqbwnjxl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2vrecjmqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsulnach.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pubpbswh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvcoqbag.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pojndqqz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2odzdxpfl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xunerndl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2stayfljv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nwxjfdye.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2emkjsfhf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ajbltaou.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swdhovty.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qhijdbug.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ioznyaqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fxbqhcur.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hathusfy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlsygtvg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldfgdnhe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wvrfrlqa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jorkkagt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yserhqki.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljwakmoy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2boqrabva.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ueivnjit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ejnafxjw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2orggqurm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iprrspfp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2miqxjlyr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dlozadmj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cmdxkfvb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dsbviaic.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2egnyfaiz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2khawoadv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2judcobjp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xkghhhxi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lnheewdk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uhmqwusn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ajxvhhby.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lzeaacvy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rlelabxd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cukgistl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2eohtduhl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2krgificn.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ogbqlwds.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wryphino.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ftzejjjh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ocvcotfc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ireyojqu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqxxdkdz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bilaxgst.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qstzktyg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zntahtjz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chmjbbht.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aijhgtlg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dmeonmwk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlxjivuw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owyvisjk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2txqmqejz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2abrvoblw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xhrtqtfw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2olpzqoap.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ptxbrfon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2milwnlfb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2edeqwktq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2konjvyfa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ifgposwf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2otrbvoyi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2zfzdsjhs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zjeiiaen.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2rbverukm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gwyvqlrj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2atqavwiq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2dnpzeiea.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ncecezqy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2shyyrbth.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mgipopyq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gkgjndia.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxmdxssv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ilhmyqiw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hvsejdiq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2svuwjliu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2codlyafe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fbrivssu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixyosfje.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mnjaefde.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jfgpgxjt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aevactir.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfrasstv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2voizkucs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osyzzykt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jiohsesj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drgzmnhy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsqdseny.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgnkgoxr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kmgzdrlp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqbbyrcc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bssecqcq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2usssytoz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sygkshmg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dspxguhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dfmygpfg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsltdrkh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qegvuypr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rlwzpbfd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2dhspvaja.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rdsoutlu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2isxkwuzv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xgfmuxiq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xzmygmqy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rtsjdtry.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2jgtvnhlw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dtouwlww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xcpofhgf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vstzsxtf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stxfuapz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dgesyyyk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wtxluzdn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2muyvyeav.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjpcxfhv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2knmblkbu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppipqmhd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fjfoaepu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cajkifuu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dweptycu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2exmipnct.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zwnlhotz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zqnnroob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivuwjlbi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpwcocru.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ltbuffgu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wuqklnaf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2omobzaro.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wjhzwzvx.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2itghhekk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2thtmnftm.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jdnlujhj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2enkpzehm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vhjgavbu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2onrvttmw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hkufitvx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ownvycfs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mtzxbggw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2woskgaak.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ewlxxqne.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cejrioud.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdjqjvir.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiswsgwz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2slsazdke.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2thzgfbpt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2waattrml.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mzqhlxtr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gsaivicx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2frydobbr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wqwdnzuz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmxvhzbh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddmmbgkh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dujovakk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2smiqzuxl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2psfbpjla.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qfwsfvme.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xiazebtp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ydjkregs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yirhyzfp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlnkjgt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2owysnknc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pticprhk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ltitofsp.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2isibkjdy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pmflwwbv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jwighaqn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tdhiianu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lirlhchv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ljewxooz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yufoizcu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uzlyossy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2emtiaids.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lphnjdxh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2niegtcgs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xpooxbth.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zomgxmdz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hitrswxm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkolqbaz.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxirygka.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cospnnzo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxyyua.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zgeqguyc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdbszvcl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jeujbovb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qpwwftwk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2btyxpywa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2bluearxy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2xftbtawo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2sqzgrfxm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xelouvvi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2piiylsez.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qdgcovtw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vpsqzbjf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dksqdtvi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kkpesldq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2puazxdim.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eorkgcoo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2nbujsaxd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bcyumflm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bbwxylqu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ncekaifo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xveyppok.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2tosazxxb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ixytwffc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2uexefqin.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pbidsiad.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2souegihf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aifmuihk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2okmfajql.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbnsauvb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2yvdvlzif.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ajwssyyz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xqdsazmv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kqcabhar.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ewnywzjz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iftlsves.html


<!-- 参考信息 -->