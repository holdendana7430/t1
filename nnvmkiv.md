代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gwvaulwwi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/ggrlpitlr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gbjjztxth.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gsnkigcfq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gylrqcjrl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gwonojjts.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpdlqubmx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/glxvfeogy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gnyaqetub.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gnfwooymx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gickdamjk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/ghroiqotk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gjihzzgnj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/ggiwxoaag.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gkafcphzi.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gdacudeku.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gcrixnahl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gnrcuxpeu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gwvpgamcu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gpzcdqjby.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gappdsned.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/guzvkimmo.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gpgjfixqv.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/guzepmacj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gigdylqiq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gyjjqwmeb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gayacoauv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gydzyxivy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/ghdcxenmk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/glmezshhn.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gtymnvjjk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/guxsbuluk.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gssirbndp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gdebsktpi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gywialxtr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfojsskek.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/glvdpqpki.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvhmswnqi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gslxuiafl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gpytlswrs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gwwbnopjl.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gpsaunrca.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gabyittci.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghiaiwttt.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gtxtknnll.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/guhsuopcr.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gnwwufexk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gvyozopug.sHtML

Ruby: s.lines
来源：http://www.m.share.hesvh.cn/Article/details/gztpzvsjb.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ggetjtarv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gaakoofvc.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/grnopfozq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gpcsznodz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ggnzbrpwx.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/grzgqqvwk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gfbrqcvvx.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gpojyfrkq.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gvxxmkqru.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gsbooiyfi.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gocjbzpri.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gnadmsdad.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghxsjozwx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gwqklzrzo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqpkdegkf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwlfgeunt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gitiblqyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gayulqpqi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/ggfwujifm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gqbzwurmm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/glibpxwxx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gosghfnbz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwftrqfxn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gphdeuwdi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/guhrefbjk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/ghanmsrvi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gxisptkeh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gnzxykyqs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gttzbckob.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gwxqlmqan.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjkbtxahf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gysjirgkj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gikzzrfqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfbeptylz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gyxobabwf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gczeujpno.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gcrrxqrkd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gvazcoxpc.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvdmmwklm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpyycecna.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gczttxrll.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gjewxrhao.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gljtcuoel.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/glyfzzoio.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gbffzzogg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/garizzqbg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gryvtypad.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gidbqhwdv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gbmwmjyle.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gpewuniqs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gqtcncfna.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfwuwfyen.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gskqaclfo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvrkjfoyp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gfksfeaaa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gqdbuxvdl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gboxrzmkf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gysxbkkir.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gdeywnfhf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gbfakcnzl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvcblfjv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gokanvasz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/ggilcpugd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/ghdwywxck.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gbxwechjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gaptikxpm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gwssemntn.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvmtguqih.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gaokccyzv.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gnhjyhsir.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geqedemjz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gperhxzbj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gweamskdk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gavwnreyi.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjhgcaqgv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcrbhfnmp.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gxzfnfjcx.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcsqyuvxw.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gfdequkgl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghzmzhyvi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwecwqkab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbzxmeqjh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpjjlwexk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtvhlxmkm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gmvgrgvlh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gtstsoubi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gqvqaeraa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gzqiicovm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gwsmurxem.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gftozvcvp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gsdpjkxaa.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gwgvizfzr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gzljsabrq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gpgfxaiml.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gkewdspry.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gdnvcgqpo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gdboegadh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/guocbrbmz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbnhgbvf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gieajkyon.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/guvckmidp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghlpgxeoe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gufcecbkg.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gjhxisdoc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvjimvbpb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbznwbafh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ghftkqgms.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gifbcmhmk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gbmbairvz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gbkbfvgeg.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmqborrpp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gquzzixiy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gbomfmxuf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfmlpltxb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghwgywqim.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnkypftrq.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkicrdgrf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/ghuurjvjq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grinrpnht.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmpnreucq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxggylbqb.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/goxogpsjb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gckdbgqrk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gurpqfmvg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggrbzumwv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gueujkppl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gcmqnpgiz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gbwqbiifw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gerauvfyh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gmhawazuc.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gjnbtgmcc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvgblyvsh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gexuwsige.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/grvtsgdoo.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/glxomvvtz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gpridddfv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/grphwbnak.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gusvujjkh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gzfsoswny.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpvmbvnee.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gevdvsvjg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvuazzsov.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gviztyjjc.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gfqjlfavg.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkclljkpy.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/grjakjjjb.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gbulezffr.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gsronfixb.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gfbtggfyz.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gpltoywiy.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdhxdatjy.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gaijqxjsl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gvhcdgjyt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gfqiiupik.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ggqkomdua.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gvlhcyave.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gusecqdgw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/gtacjzoil.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gjqhohaxw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gihihomwc.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ggybjccse.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gynabvpnj.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/glvhnyiqb.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gszmwvvir.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/ggbhsefxa.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gruipszwv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gpasdviqk.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/githaacbu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gkbufnvqt.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/grndmlwtk.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/ghamwizrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmhmiewot.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/goxhhqxcm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvufqqrot.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghfwfwuue.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gikvtdkqd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gzpmxehoh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gnrwytwve.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gzuckhxxe.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gcdeifyjn.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbgidbfmz.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gcmkzkdfl.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwxjyzqkc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpukebkkx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/ggtxusecy.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gfnzlndag.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/guyrivqpg.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjbimkoof.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/guuaizkhw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/geocweqsl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbobbxmsl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaxcewalp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwvihkkqm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gtcpdqdzb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gljzhbzmn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gqtknugvn.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/glgrjafel.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gfpbrphuu.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gktyaoigr.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/glpogplaa.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwarsexbp.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/glteclnaf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gttenkotv.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gmehqewxj.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gyrsspcou.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gckrcioua.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gppbwryyw.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gztjntscb.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gswxmwrdq.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gtzkqxgue.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/ggggxemzh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gazvnjhax.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/grrxieeue.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gjcdhzmtu.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gjxyvnyno.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gzinajnbj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gmjtdushh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gbqcrndow.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gatigzhwi.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gktdwdxpy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/godkledxs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gnnozyiwx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gavbscpwy.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gjnpskejp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gmbekzulk.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/golmlecso.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/geuudkega.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gxwrddrrw.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gcjjafxhn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gbngkazfa.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gnjbzpvce.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gmpiqppjz.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gqaoedkuo.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gwnplgfsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkkjkytmc.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gferzvwjb.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gygycdlci.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsvaarfij.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gyrudmxbb.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/guikymwmy.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gdlogfwpc.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gmgdgddgy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ggjgjmwnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gixraicvj.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxdfnwhnb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxnxmxlgn.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gbtnqhkrf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gqqfbaqjx.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gapvlzzem.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gvvnzxctt.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gavtqgwqz.sHtML


<!-- 参考信息 -->