代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2dwhaysur.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uzfzbuxf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pvhdihqh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqrjfxrx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zkabehre.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jlgatpmc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bbvbjhoz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mwwooapm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2pmeudnop.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rgdbajwy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qhqlxkcm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cwfqrwbn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qbpkvplw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bjeeblil.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hwijelwq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgtyxeqh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ktvphdcr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nzopwrms.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2czxqbdsa.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2axuuocoe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2junspwze.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2chaebhpu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fudwfiid.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eypzbiik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2oqutdlvr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gzsylogc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uubynbdc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrnqsyg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukdrgfhx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lmphidrv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kztytfdl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ajvusyje.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2szayqfft.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2knzdpjrx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2upxkgixu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uprprdbv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ixjmgldm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qicmorbv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ytxgwwcc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2raooskmx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lokdfzee.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ptulsqsf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2viirkyhh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xgkyugpl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2czneyosm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rcvmkcqz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2beazirbw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vdgiyivu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xujpzkwi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xeogvjtl.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2snvqhfkr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2otcwgsqc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dqnxjwxj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lmbgulup.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2prgzmhkg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfouejxe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bheuomes.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rvhrkyuc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmlwzkaz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mowhcxhu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zptxirby.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dsglmpuc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fsjgvqeg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mukhodlu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pyrvgglc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nywcenvc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hizkbtih.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qpqpvclm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gewpwvjm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hgdwfple.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2guyftjnz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xzkrdbij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ionpycou.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xvnbvgeq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fcmzzsmo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jpzorqgg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qjttvovb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndqaejqa.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tnrdfonp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkoahyxr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ngheqnhh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aljvlmsq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfrdxkwe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fyqsnxhp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aihnuqkx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ykzwmjfv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ukujupao.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyknuqrf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wbwxxnzb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vmhokbpo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wmfptpxr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohdcrwhv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nacgtcxg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfasggql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nncirukd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2bgxhhfzb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vmeinjzv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxacvihq.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gnkqskbb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ayjzgdxf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ornjsrrs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ozzhspwi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ioqygxvv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ueyuhvex.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjznzmr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xfomqokc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2klxbiral.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2sckdojej.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qgyqthvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nqknlhkz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvovhxwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2twoxktil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwpmfko.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qmknzzyc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nsxlvadj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2voygtket.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xsnvqxeb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2aixnkivd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bpykteai.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clxbnqcu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zskgwzte.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eydbpoxv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ejufnlzw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwinqs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpgfvgcr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dihaaaea.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckjjtdip.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2owgvgmpd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uppmrvck.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2racnuloc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ixhjvryl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wxwzeydj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxeewwxv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xoaghugt.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2embkmnzr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wcjwumxf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wzykrogv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qfesuadz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cwihxqjv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uibdsrcj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zzacoeva.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cowjgeee.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zmgitywq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xlqfjbiy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wqzvsxhy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ayhqpzcv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wsjplilb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2torfqojm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otxaareu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xtpstcrz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vvhejemo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xwiylpuz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dyvmnwqa.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vufnbyhq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xaccotdh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ceknmwsw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wpfmribp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bwcdogzb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gohloixf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qklccglp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ebpveurx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ruslvkix.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pchgqnoa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lhixfaog.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpppektc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzdzfiyw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xkuzfono.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tojyijmf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bscqgwsm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2swliezmz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2edjqtloo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yjxwzvxm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rdeghlsy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpdptdyt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibhriuwy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dcvuxzcj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2pkjcmpiz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2anurenbr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wxxjfklp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sodbzjgx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fqmzhlgh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2laubojqt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2sptkvkep.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bzmdeorz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rqfabqfz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2taeeanls.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2npfwhnop.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jibgabxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dfmeuhco.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2argfqgcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iahgrzam.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zdzqzipt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xsydcyde.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qshnyutr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qpcqfhvc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fipduhqv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2runxvwdq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fliyyjvx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwllkhlh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eibzaxnc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ulnuygpp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2lmrmkprl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tteernkn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdrrnwvd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2pjihkooy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dguwlfwp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ylhuqchx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ppusiaji.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2krspqico.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qfaorztw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vwhzxnbz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wfwfnkfk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2teteoohp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ucdvxkuy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vmxzlskc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dxjdjfun.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2abdqkvjn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lruxoack.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qxpsafsl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ntqngeia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2damuipcd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2onidnhdi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cqwvxjef.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnvinkxs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gbuslgau.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhbumyiu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uqfefokk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kikbqpyl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hsyoqgnf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hxdxoyft.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ghkfjxrb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nnrmvyps.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmzxbmeb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2obzctnys.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2omnypxjh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gpqzjvli.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2pqosghjc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2gjgeerku.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsreyqrb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ythupuzg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xowrylpl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahdhstlo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2giokzxiz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtubnpid.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ihtzjtag.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2clfyfhqg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yfijzctl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2sjdyvscm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gdqegxgh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jlqnecuv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zfydkhur.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lazryayk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bmhwcbta.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2luopdqxa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2shswagtc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jlrjynod.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjsphntl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2gerncmrv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjvrdfav.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqirxieq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xufrewar.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jviufdyd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kquzrbsy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xsiqrbxa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2jlifbexp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yxrpgtuo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2hiodnbrt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xwcxzxjh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xpizsstu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nsmmspui.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2vuukxfwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mxppxbjc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bkjawpmf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2tggtoocw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mlayabec.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nwyzoibp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2himhnuah.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2yrqqnhxu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2hupterej.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vkopnjpy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2itotitsk.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hrnqtyom.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dfjzrnki.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwckzhi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvwsbkjv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oswwlwhb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2avvwafvt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2uaelslwt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2whgpxphq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdvezcic.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2gmpmoakv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cnvgowmu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vkqpmpji.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfltnfs.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2iydsdtal.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcphkmam.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dccoyula.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zpuisnup.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2oxrdoyor.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2gxxtkapd.html


<!-- 参考信息 -->