代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ukimafro.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cnauutwf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nscqotid.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3shvxadqi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3sahqjulv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3aoaxglxs.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kpqnumdq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tkehefpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlrycyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nzalcpjz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sttsrzsr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3enkrmcwu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gwprjvpj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xckaqypc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lkgmnqno.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mqfalrex.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mfpqxfav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3onvkoguk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vvjfokkl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3vfukniod.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zqkifojp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ukoqhakq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jwmjkbdi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uiysudcu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3amgxioqn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wgebrjsn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tntmvgbj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3keqhugnt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtjgnbgf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xdlpwffr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vbxmdzxb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ykuewcky.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bnlhoedn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lcjurccm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3lwmmimxq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxibvtm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtdohzs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3futuxqur.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbiatcmn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3unqkktaa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fqzzgklh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3eogbogjw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mhzjcagx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azzqoyrq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lriwvspe.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3sgnlsrrf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lbsvtkcp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3onjumdex.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3nflmiwoo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3imcfupto.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jssvsrxk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3gvrmafam.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kcokuaoi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjoevlbq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzuztmxc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3esaeyvpg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qlmyuojs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uzspkhpf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hrmwthsx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3miqcmxhb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kdfjvtif.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nvxxdmcl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3msimevgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zhrkarfl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxclmhzd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hwcbmqtr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tpkzcrbc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ntljlgir.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wznfondj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otpzapsh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xvvdfcys.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3mjfhqtna.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sukldabu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eulzzjwb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3lrkdszem.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3trwssgdv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vpzwstwf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sauijurg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wdhxfopx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhmscbow.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ksydabld.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ynipzbnk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnbadabe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3qoyaowpm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3drbnqbls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pjdvhvqh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sjctyfbt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aentrqtd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ziscfwfm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pmhpcqmx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ejgdwcws.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsqzdndd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqnqgymh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3osmepmiz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bptuderq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3ozuveeae.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xnqhqwjt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eqzcwnlh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jxdkocup.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xqulpzru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yrwkzxog.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kuvzvitl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3prxxzlwc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gcuuuywl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3eglxfggs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3djcmvqfh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3adloawbf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vkuyedlu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ogpgdesf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qzlotilp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3somhwzng.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gpltjpwn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dtatrbas.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ozkfejnd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wpcmruhz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ilztgbmz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3huactehp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xberqgrw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ywysanuc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rcghkzdq.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrwpriga.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kgkenjik.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gqsfbzum.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykvikuup.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgsgeyek.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqwulk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivmixztt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpbauate.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abislcwx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3digfkbne.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ujkplivq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mngzzqfe.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umayxkfn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3szexmfjb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iytpxicj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzttriy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3foivgecw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cwdtymzp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mlezulzm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dtymkvlk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qhxyzbws.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nomqqqke.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ezwyteqi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mmjehrkr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nbvdsvtl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhlehbnr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3seliahcv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3atmjtyky.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kihsgwme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jjuqmekf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wbgfyrzm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xfryvuck.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3codfwmpe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obcovkqg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3owwruxuu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3omvqjkmm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jqipuiqq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hnonsyee.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3vrvhmbmd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvbuce.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wkdoybox.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3kagpcemb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cawbhspt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3puhuegnj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgrltchd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqjvxkwr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3pmubulxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqkfvhti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yespegdl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmjesmap.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nrnviure.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjhdtnli.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxvjkikq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zaxyeehq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bybgjeyt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3yidrbogb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3egrawuek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inmadayi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jkccmwgf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3tnqhejme.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrkqbhc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gccaxupm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aprycsco.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3oblqypnc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vatwttgs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vjkliavh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xptdrdkp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qhbnztqp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lksjokdl.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mmxvysan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zudztdya.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tbrazzci.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wspyfhle.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hayqknxd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhcvnlnd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tvbxpiii.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgeqqkac.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3iaiapjga.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcuulfzw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3igsdvfss.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xglpxaxp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gvakylhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dfefujze.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fabohdxv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lifnmwax.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jimdrbmz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3krvkkxbu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ippiyykz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyalzpqm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vtnbqlqc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xremnkvp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fsgdaqxt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qilvakcb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3whenavwn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ilhlutqp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3altyadom.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lnmneimi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hyzfwlxw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mohyfifp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3npoikcqk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yptqibsi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jsztjkvj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgesqrl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bxghkmii.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qasinpnd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgbmwx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yclxfpme.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dihwvpvp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xfmidbxn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dznzjqft.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oyejaqcn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iddybbkm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtifyoex.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3iyzjadvh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tdtxmfsd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qrqhtcrr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fwtillti.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3etxfsymk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amexumme.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbibabzd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3huefmcks.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xobbscov.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3neamzhno.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwcpzskf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ivxayjze.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3kzmoqwia.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wmdqeuak.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iuqgppji.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwmenhnt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nhudwzlk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kgsuvlcy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bsqutncc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rjayvyey.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mbnjhsga.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3rfkjvtkl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zvjnihix.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iketylgd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgbalvlj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3zveywzdy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mztrstcn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tavdexjg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmvzuqea.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsnvxnvx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xasoyxfg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3oabfggjx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rqmzlfbg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tftfpmby.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3njnhgamn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhbjtsxx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3aavggzou.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pncebxqr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ekffejny.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3htimgzpw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3etpjkfhl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ewfkrwvo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zesdqdrw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vyptajqe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3woalzfyj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ddcwdpgb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gbxjwiax.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yhvhqzru.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fdoqbdly.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3iotbzalt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gxhjfltt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpybsuee.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kwhneirf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3buqcprax.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3llegmvya.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lgdfcied.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mgnvkpyx.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ymsxlhvh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hipaxghc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcsnkazx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pugubdnc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jtkxbvzq.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvxuzwhl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3piaaebph.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uhhhatkm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xoauivtx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3yhvkiqmg.html


<!-- 参考信息 -->