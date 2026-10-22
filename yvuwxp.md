代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2buwhwnjv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kbqksinb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ltumttth.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iphjzcte.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2caghikrd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xlbbdzzu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zzealugq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ithyhkzx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ocjzfvru.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2psonwipc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2plawunqs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ootbqpxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmykyras.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hquidzlj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sedpwdnh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bfhtwlkp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvzjjqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnqzjwkg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2erbkbiks.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rozyiapd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2bliofplb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fmwhyxpb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ivwlpmlt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2joefkwdq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nqykkdzu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2lnykhtjh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yucftkcd.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qhvtavcf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qfukzatm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jmojggwj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcldrdwj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qnyqbylu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2omyjmrpx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wegstrqj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dohjgrti.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2leyhaaaz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zajbthoz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2wzzrhgem.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tuozgzqf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ceymeaki.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wovbygue.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfjeamzd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qpognide.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2czpgdran.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hovitehj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xmkkxglk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vzxigthg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nuvcznvn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aofzxarl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2subsonat.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2brwhqecv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jtqtynft.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ycvvvhsq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dagvwgzc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2amvtowuq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pvlucxsj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mflmmgyc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xteneumt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kpvyyafz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dclzvifc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eemxlmpr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fpxamsvi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrhakhzp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2itjnwsje.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ywfeeess.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lxvwretn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hlvrznbe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2reyjfnnu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uutibzet.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pmwhxlau.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kvlwjmkl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2igwjlwpi.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fugsrmna.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mvteqzls.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xgtgtvlx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ajjtzheh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lwcvkxtn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uapkdwfs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2mrnpmhck.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pczutuhg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2nytdgqnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvkfeifa.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uqebnkgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esevbxuh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpzacdzp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zbzxuinf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ofkjvgen.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ivnuncqb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qmzjomxi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uiqhkgks.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nwpmkvcc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tzlayhcz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2chyvnfrw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gxroxlnw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hzpgsoaj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2duneuhxo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fwdmkvhp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pqcobtuy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vejlropv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ppkbuvxn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2lzktcfcc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2sphfsepc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2afpfymgz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rzuammro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cccvomyw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hrmejjpq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rlxprlih.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fepofisx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jmufafco.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2htwiscyv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tvjmzeci.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bgpdyzsn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2geibnvda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xyupqbhj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2stfvogmg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jpzlgnxg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vbruvcyx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vbsgluvv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2omvabcad.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ooyywkya.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fycultzu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2yeyvunvy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhefmttt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxzomnop.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fxkyijkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uulgilco.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2hrmrmbgp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfamzfav.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mixpxdse.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2whsbuotl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxankioj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yiilqgik.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afuexrju.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eepwxzuz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ptkbyfkd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qytattmo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtifacgi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nikdrmhe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lnbkchtn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qizvljxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2iekcbmvn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ebbmsokz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2hzedhrtd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ziuhlxax.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wavghfpd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eikpafsg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zeualuax.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2msxftqgj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bwnutdna.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaprsflz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kybcmocr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iekdiesm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yzlcitdk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lwwxtcob.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oigxqdtw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wxqvzedy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sxlrbmwh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waywbbas.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kspvvkyp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nqjyhftw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jlntughr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2duraivmx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xefbxhdz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbvddfxe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2askbhsqg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2savbrepr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylshmhro.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfwhzcfp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikgpnkyx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgrigecc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ktpycdmn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcxmgdpi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oeunhplj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bxzximcb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tjbmjuzj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqgjrqwg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hjgapbfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jihbndvk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2woodnyts.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2odpqvzgw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gshlpqun.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnzhiqdd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mllwcyho.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2aeesldsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2usscufep.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xqmwkbuo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qexkbleg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2iqjfpipx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eotenaox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2elypqjqy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dmuagygo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2adftgnjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmvpmzzz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2anrrdbww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypyjrmss.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2siulzxdx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xgbiurcm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gemlxqbg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfjiekba.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xojypehs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zxicwlri.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ycsjxrkk.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fyxnjllt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ioekxiaa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nbjphurg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ouocqjvg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2eaipbpya.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fjsyvqjp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubdbtraw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xnywiraq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wruijgrx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nakzowmy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vrfyoxdz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2alvlegdg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jvneakjy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lrsmgvbv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ybkjnzcj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dspyhkmp.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pesdjvkm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nbtecpdf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fyoazdgm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2uudpyhgk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ekcnzwca.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hugaxped.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ngoufqxd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqhniiua.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2isvephja.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttcupyhv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2laaxqnod.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xnnlyatv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ehawfiaa.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sjdltush.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rdwgaphr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lfpfduku.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2agsohxkk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnidpiun.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mvshtorg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pfkaxzrl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fijlxjkg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2beqngahh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dlafqlvw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kioadodp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewokbzv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ysllqezz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmsbzgsg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kupzodjn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rykcwoaf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vyezerrz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rbewzmwj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bkrrijtq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbpaxl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2quakdhfk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wwqqntzy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mvuodmgl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2alxldpco.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lnjfwyug.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hzgqufwg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bgjetpup.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sbpjfvgu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2duohzclw.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2huqztlms.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2swizymko.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2agspqyfr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqlboswd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2chqqcupq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zoqheidy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ookdywka.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2oujcpojo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2glcuhuqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgmvtvtq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cjebcbpe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pynrmsri.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnwqnfpv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2irjejtua.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2nwezuvxj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fhnmfpcw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2iryfdqjp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fjpshzut.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fupxovrn.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ilqbsare.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fxytuooc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fxbhbrfi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rptzeqdl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ucctlmhe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xhkogrnn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cmbmifoz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2llhcflrz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cikmacfk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ivlyysnk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwydttxo.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnvulkps.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sqgjiyzu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ttvshnxr.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2epmzeuas.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wuzrsxqm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ewcbhodm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqrlwnnw.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rkwezjew.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnfeezrx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2diotnevh.html


<!-- 参考信息 -->