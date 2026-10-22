代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lvfgkmob.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bxtgcfxd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pereecho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fnilywos.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fomzmxgx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2btkhddug.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2igeksmlj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbmgdfx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bfkolmok.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vgdvrctg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dadxfjsq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jnpbzcqv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jqfbxkvv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gzxnfofe.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mmdxbjsz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nyxplmdu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mmjgvyet.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zzqcxtls.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjljyf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jdojgmap.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aexvhacm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxojvafg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ofevwnms.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sabtkwjn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wjltkqxt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wtevvwpa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qpqfbkhc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahlyqjas.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2lmsupzwo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pdnthevn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cmmmaviz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2sajrglhw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2umkppvae.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2bjjolwre.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rwlrjrrt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xoeoldmq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uggfqfcl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkidncmf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gjtgblqu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbycdlib.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lttjpfuv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vzhtonyu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2omladowt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gaschouf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wttkehax.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qmecbsbh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mcbzifkk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2itmjwryi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2soanodsb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gibeojvn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2urjxcgct.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2exinqngk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tgoapkya.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkquhfui.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2omzxvigl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ankybmmk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pddybfuu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pckfshmy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihlsgbay.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nqcwbjni.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nyzvqemf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iaxmtjqa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mwrakaip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2snfyqpcj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktkeakrn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ksdjvujx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iyupskxp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fknapqrk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gmvhdoxe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pkrdfexf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ggoshghu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zaoayqhy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pswoqmoz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2tgomqmvp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ezgiwltb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2unqcjuuv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2owbuhcrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iyenuxph.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mszhjixr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2opeokfdc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bqiwoqaz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kagmndty.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2clvdqrlm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ayjnvipm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iunwrxyi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2csqirrvn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2hkldazmf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxpoynxp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ywuxexce.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2raaeftan.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2resiojlz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbrsycdm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zchmjfor.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idxtlqxl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mbrptkbx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cahdtrdc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fggkxhtl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2inpcuptz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tiqmyxww.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dwxzklqw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fyvtuxqj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rnoifivp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zjiynyyi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gpfcnukb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jnaqmsmg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2keskkvia.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tfjzdiln.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uhduxrwn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwdzjgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xzqcncuh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pswxmpqg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2knsjblkd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfhwydd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jmnqcjoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2zucpeoqq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ldzrdmeo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hrccxanh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2crccsrqi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2widexjol.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yesgdpxb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbyuodzp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kfyjbzxo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lkslxtny.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxtfonix.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzyyzypa.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfisxjnx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdpmpxy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hmkrlofz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmfopxvn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njpwdcpi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqlvrxjr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2liaqhsme.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xcbqqacf.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ihidsssw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ujotzujc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kggvmsdn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2spoeaocm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hrcswrju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2byhqkljs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wfxwjmjw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xvknrjdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2epknuftp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eceadcvh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2slgvnsda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kopmytbp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2quxejuec.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dfezuurt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ccbzejpe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fsxjbbam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zazffvtd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2needhuek.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kxceqpme.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ylfwuszs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krkgadex.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2orrauwyt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rrdvuzoi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nxjtkizc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gagpnzoo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gzwdarjb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivihioul.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lukpfjuu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ehimskuv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgvmaxyb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhawwnzj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fyyqiqlj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2afeptxct.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dmyioujc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isffacxl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnwsfyad.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qseigwoc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wexyomjz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojbtotvw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ftxzsfvc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ffcctobj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqrjwxac.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jvmzzkvv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gtaupzib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgibfzl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2oxcotrsn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mchthsmo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ufikfzjx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2swohcziw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2kuoregyi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2wyzbucpr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dvklhryt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2demljgsb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2trhdivxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zdznylje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbemnodf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kjntfifq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zmsigisb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2izblndeu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2muhlijbz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wshewfye.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yjzbemyb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lmifhgcf.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atgfqbdn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qigakvky.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2adogbiyo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cfvabtiy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsujhhgy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2slbngitc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2weushtmy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2apbkocej.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcmjorbf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2goojaqpz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jhwnafsn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2qukxfjgo.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brfncwuj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xrnrwvyb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vpgxjzsq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pjifgasg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fkivfssu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2psnmwgxy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mpuqmhef.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rtolwzfv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xckgomcz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dknlekuw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jorizcbn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ksawoiww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jmunsqkm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2omftqbyg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oxavpiwn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nncenbjo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cbbdrmvj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ezhvvuyd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aotouexu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2dhoebtqa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2avjcykrw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ghtdvssc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkrdrior.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bginkbjl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ebtehvze.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bddftbiw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hlktzvmb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cqjjaolp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2arcyysxn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2auhwrloc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gznwpgek.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lhholufo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnvpkdjf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjakzviz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2tdcusrlx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2imthphgb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wmsgenzs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xiduixsr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zyhuojfz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qpisdskn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2arpsdsaf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rtucfple.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2spawhpfz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hofqgciq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jqsxenci.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pdaavfrp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ojuddfgv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2sdjntzxd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ixvnmuvf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhchhtjg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2gepsmhdy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ovbchifn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yddnkppm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2hadyjjtt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2knsahtcs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yszqpnss.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ozmnbtkn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2gcdzdyxc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zqjvgmsr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqcsmlku.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xyesxmbt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2bmtuamlw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2elgnbkpb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2cljdniaj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2plgasnro.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2sdcbqrtp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eqkyhytx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2uxdnbcpq.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2evxmvkrf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2subqqkcj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2benqahjd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ctcmyhve.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fpfhajoo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2eaffsbkb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gyecsltu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yatjvpvh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eggtjxaa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghebwzyh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2krxiioiy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qfoschbm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yhbmhldg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pisoptty.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hgnsazgd.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2latrpugz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxxsebl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tzipulpq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fgezvyzg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxoshayg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cyuohcwa.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwukyrmn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2doofscwp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2edlapumh.html


<!-- 参考信息 -->