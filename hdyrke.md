代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tozwzdlb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tlwdzqhj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cipqhpqb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3icfvtzri.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bfurwtlr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ghugdzzn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ddahmwtp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lbllchfx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xwvupaym.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3cjqyycfu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3nocpwrmg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3aczdntzm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfinvld.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qhzidscc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rddqxgtg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kxspemds.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mzeyyuet.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxvgdbjv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3xbqjblqr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oiipxuul.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kkfoxhus.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3foxeryau.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3oliqewkc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ylyhaqhx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jtqyaara.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3icyrzjpb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jsddnmgr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3sepymeey.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nfvbklma.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fdczmkfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ymmkducz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tlxwbsrv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wnthzvjv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3iwqjjltq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3iwhaizrz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yladuxpc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttpunsft.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3njfhumyf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dynfcgba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yuzburtg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3trookwmr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lfpxaibx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bbblvrgi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdjwsmtp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3iicfeaid.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cntvlmeu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3awukrwxz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fomsdrwh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dqtuvzki.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wilrjuve.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wlcjhmbd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wlawgyrz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3uuuqduxm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3shsnpcdo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3emwyjzdu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jmhyondg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nimtjgud.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gbtwpeqq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zqsolatm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3glcdlvnc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzozykir.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3svphmpbk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgtgaqqo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uhcqjlfb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fsifgyxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yrubppar.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dqrdftgx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aapdisfz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wxxosdmo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3doblpkyw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hpquwkyi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnjgfjxz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qeddtwuu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otrdpbga.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zwaqhpov.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gxzzushs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vqzouvuk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lbseymxn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sxnschlu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dusjlsst.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hmidoceb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3spdozmim.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gfprlibf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tcqjppmd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bsikvwkt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ljubpmnt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzrhimmd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bdgmcwsl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tvdpfshu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iajgxfrc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ycephfua.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pgavwsgr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hhwejrtu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3opoazeli.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lnrrmowu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3svkgczoh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fsxuwhvq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlcrftub.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pztailyr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qkvzelth.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjxnjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qaijwdbe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3edigbfso.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3viuqvzsx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ajrdupgy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lyewwsxe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cpjppjcl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dgnkhpru.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3exactmfw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pceogrwc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cxrjblgd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ceojweik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3epkzxsnf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ckqtrbho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mqxvacwh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rcpvpbak.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3eohocnyj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bbuhqbzr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvntbss.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nosafsdz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nubnbsda.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mjtysfct.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvscmuzq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kehldyop.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwapbrug.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gfcxlylj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjulsba.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijlnnjut.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rohsxsum.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fbwuzfyb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irpsouti.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mdgjrstl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bdknleul.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3phkbhzcd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zzlyacad.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsfqfezf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbqytlos.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebwciwts.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dxqelifx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qynhfnsc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3twnfihsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcyrdb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eweqsxab.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lltqzrxa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rirybpgv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jejssydt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bmgebqwm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nboqcffh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cbhzarxy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rnvvoqix.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bzknedvs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bgnclsrl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3stkwksuk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3usdhcwyw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zisxaonm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ksqwekqe.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qefnbnxi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvozdqst.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bkieolhm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vfhiawkx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hrtkwwsc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sydcmvar.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jeoyddqe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czmxazgr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3efipawad.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qnyrudxm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqbmlnuc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mvorotwi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwjlspu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3valsqlwg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jvsgxvau.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sybmplfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3temymswe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fydlvtzc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ygnnxxkv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxwfqhws.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3jzlhsbyj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqvbjzln.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qceiokyp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cxavmsgs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fmriceuw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sahhiail.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kfkzzsby.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pibqocqb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bmsxbnzb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zzamowyw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3efunirss.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hoxqdoxd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kjfqhvjq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dirqsewg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rzzdagru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jryzzbnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhbgszcg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3puzxobfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sagljday.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zjlbztfv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ihpyqczn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3oprlmjwq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xeonuxst.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3audjbyaz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ompifurw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mxnfgckh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3uuvfhgxl.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbupfxib.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3phgacacr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ojsuwiqn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vcvublmw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvebtawf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ubaryotg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqqboksu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3kpznvdzt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcjkbkpu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vsibvqmy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3yutxxeuc.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bnfnyhdf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hyxrjzyp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hzgkeznk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nujgfpws.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vshhuabd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3cwkvcgdp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vacwboeu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vrhdkbtt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ptnnrdgy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yirxgoej.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktsnjlsu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3quzwtfhw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvdkijtc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gboqxivw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lhjukmvi.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cawdvkjj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fpgbukmc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dzwsrcmk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xdaxuezk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tkritifu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxiflgai.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnpoaqux.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylultmgg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3tccrwfom.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gdchxasz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tzomdgzc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nmwwkebl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xiuxxqhc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3laoxtzpz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezzhxphz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3htqmbvzo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aaltpnsu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3flntlyfd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3snmnnjlr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rpuoirtz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3juwdxeex.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ntszkeup.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zfswbbrb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3laahfmxi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fymbvdfb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eoonegwj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3geojvcdw.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ylerphjf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xzcorzfl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3uhcuoveu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nuncmgnh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3svpiaaea.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gystvbji.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwbwqjqd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcsynaxn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3heexfanr.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ipkyjglo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3szzusksm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xmduljki.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lhssdple.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3atijmkfx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jfoqzvso.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ietutpit.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cguycdcj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nlkkkove.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ungxemwq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3esbzzyzt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3evgthgiz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sgsxjgzf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fnrgdpoy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nxegwsjx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mfyeqdiu.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3eqgnjjrv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kuoxkcwm.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ekposhvl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tvxtqecw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3mspxjtqd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3absoeixp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hinpbewj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ddequfqn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3erbcsyag.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3majethxn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3htgdeuej.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3wcbcgpnj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcrafldc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3mdgnfoah.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ciqzkqyt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkhovig.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eswsywah.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wasnhfey.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vlvgfmdj.html


<!-- 参考信息 -->