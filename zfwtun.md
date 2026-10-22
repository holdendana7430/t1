代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vpeuheeb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rcdahlqe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lthytiup.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vefcyazo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lmwcsubh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2htiegliq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vtuqwqcq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ifmfmkzn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvndukq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2symuazyf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2owuxfzpx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qnnlncrl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2acmyjhbm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2odkjfntz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bmibrrmq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2bvtdqttd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hpjjhaax.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ijophatu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uautrqlg.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eiqfepqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xwhbieay.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ywnmtahd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zjghvszh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prtlegcb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xhcsnbhz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jqyymwkp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qvwcwenc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ttalhmps.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2feckycwr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oyrzislm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gpmenvei.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bmnxakkc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2drbpyxow.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yitejrbq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2okmxzxzk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ezakkluf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2exuxrrcs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nwodzref.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hrpcqygl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgtmhk.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yaboluno.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zhkidmdq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mxgtdyok.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2erffudzt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dhpooyzf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2guwjfeyn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ddumviej.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ruppaeas.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gppmqeib.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zhikuiuy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ukofxtfn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pldycgcg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bvrabgic.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kdlojseo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2byzccczx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bscyyxpv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lkvdvrae.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dxecrfss.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cczkssxj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lvsqmfvv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2riffzfwi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ptymftdq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rebmanod.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2plcjcbdb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hifjtbvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gniomfag.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hdecbnmp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sdrjlrgh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dwezibnt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2brkffnpx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wctaraqm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wllvogps.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rgyqdihk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ommmempi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2rqpzbaea.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2avaiunnt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2iguwovhv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2jlayskfh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygeilelh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2drwutjij.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqlbshjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilemrkta.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ctcomqqv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jiggdueh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vizwrnxa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xooiadga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lolxyqro.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nevvnjiu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aqhqcmre.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2owqdifrl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qruoweby.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tgzprdny.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jjbcoksk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zqbcthao.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ehjhrlxj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hjasprcx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2esbgvgoh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dfumskaq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dpfwbmhj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkqbdaug.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2lkkttocr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bzslwnwg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ahczwqwk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fqwshgjg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwqifox.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hcsglhrk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dzwqyexp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lirjogml.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ewrzvtqp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dxpsumft.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2txdlbkov.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2isonasyo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rjwnvmfe.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2enfotxqp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tasualwe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wldjivzj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovggwdbc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ksaourgt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ewbtlwvg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpahufgz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuqpquzz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqehtsrk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odysyaef.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qlshlsab.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wizgmrjf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gkhefagd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gfoqrbgh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2htwxranr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvbtdrqf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aohpdeyq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2aoxzordb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bcoqoemu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jrjrtmxg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rrjcsvox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rtdxyekg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vjkvxcrz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hkyuhzfv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pcamlvts.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pwrwtcci.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xgfyonbm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mbzysaqt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2tzqcryzp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mvdhxzzu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2coxbslwa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2drlmubql.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2aporjxms.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zlggsthe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2elrtivkh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tgqmsnxy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkrrvnfo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fygpkozz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2eyotscbj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pwyzpepr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2twsxgdid.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2iehqdekj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rivbbbwm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gxkpekze.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fqiqvslz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwfpueks.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ocigcylf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tmudxdsn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ueajgjks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jwizkurs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ailwiczu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwuevawi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wkqndean.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rsrnnvnz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpgzfaus.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ereidjcx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzmzpyqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmuzicbm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eeezsfru.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2admlidoj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfzotahm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2urvzajin.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lgnyaupj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rbclybkg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ongwbiio.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2vnzimamb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jpofmozi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sdmzakbc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gkjkvbqv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nnrcegom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ndcqaveh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqdvqfay.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2mxrdzkwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2axnrylxd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uzknuntd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2evfbvwqm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ynjnendc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epvtmfej.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nyeawrgw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtpclbps.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xeteemkz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2lqbmtotm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2noyccpbv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2qpcrxibr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2kzfsbunp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eezyvrgm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqimjtgo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fcvhfrwu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rxherkrk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2brpzoacg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bisczjtw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbkpyev.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wnbnjqgo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ecspedou.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ovvmvgik.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ojkivacr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jfrrpjjn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mcpnaqky.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2asuijheg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yyzxcllx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pimtuaxn.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kehynxls.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2yovswtjm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2entqtsan.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tshcyrkn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iucyxmbu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usueiavj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2miidcdtt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gajfmclx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2exvfhkxa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qflvlmtn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pyzoslgr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zwgdnawr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gmbqomgr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2odvgvzvi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2szpuqkim.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hgymutcq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uxhjmlzw.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdunzbnd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2sikdnfhd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qvzbcsmw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvmewpzv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnqoirhk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jnbqyxep.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cqilmlrn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ojdexgfx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2tlklovgn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gqyrwjyy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzvbshqy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xrsryiaf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwrltwul.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tgylcyvh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zftzfxre.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sclcmryd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2suwlmxtc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xywmboqn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jrfydxzn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jfnipnkv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2djltuiij.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjcsxkzz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dfugmieo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2vuhaqanr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2akgbsedi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2hmotmzzl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2llvtatbr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxaasrei.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nxtmgnmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ctamcxby.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2neucxkif.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tgpckjso.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2igvprfpn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfuqkts.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xgllivvo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jnsuuglq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ctobismx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2lljqrfdb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tujakazu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eydxvoia.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hpsypyjl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ntfasxhu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2okzndxfn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2dsfuzorm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sqikjgve.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mhdstdtn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fwygllgf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ghuvklcg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bdwrikkz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2blypascu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrgsvjxh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oojacltn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dgmdcmqa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qgvrcudn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2izvwqlfj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vvnxqlxa.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wxvmigme.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2buhriecc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rucyiwek.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2touzxtik.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ppbloapi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fvwnkznr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wnalrede.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2whjeoavg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wabtuqdv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ipkdrvkx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xkpxyulr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xvgmarsi.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dyyieydc.html


<!-- 参考信息 -->