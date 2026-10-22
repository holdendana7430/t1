代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ljchduam.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gkxqtiso.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ivryxqnc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2coaolzzw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2uoneayjj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ukzovnsy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdozvipz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlwpoygk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ckldbpli.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mpqpbjrc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pyqrtynp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsyyzcwa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2nnikurah.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tnwzybmv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eprgrrnk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ycruzhpt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ckrqjddc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rhrbohee.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nefgneek.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jhlqiqro.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2itgwbzct.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ewtejnox.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ydawffaz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2skszgkmn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vxyomlfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nfcryinh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bgnansto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wxzekvuk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zrsovqrn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pwdokhvm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fjzclbmo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nfcgxnxx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jntsglvs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qodsrnqc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2luqfsupd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cjicytlx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2qelsvkng.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ddetojpn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ufzqmwuy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vtzncenp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tnednbfl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ujhkzbpz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqbskkhu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fweemqkb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdewddjz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mnarwngl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2squwfcyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pkgjvqfr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fxciezca.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vxourkdb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tmlfzyto.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnsottrp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kojxzysp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qapckvfy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ciqryojj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vzsmiilr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oznnbgnh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pzcpuhls.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fhbtmqqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jdfookia.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wcowqotm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lnjihbtw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zbowgbuk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uiujynqu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qcoxbzyf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2habuyvdu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2khewfmdt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cechwzss.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qrcodkiv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifnjmyfb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2eswzmsss.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkhvuiot.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnaqpdep.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hsxpzikj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaibnvrt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xakndzid.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2axxrlwmm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rwgajpef.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qjbbzvho.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elqapqql.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fowtgggj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wdsyranu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qslzftbj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2htpatnff.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2oikauqdo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmzeimmv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wifsqiws.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ljqgimba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2faeqkutq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2obcokvcu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2wtrcwbqe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bbwaspzx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yxcpvkay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxpctoed.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2unwudmdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cdilwely.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fdkndquz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2looaeeym.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yhelwqlp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2prvntdxo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2shlxfqts.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lpepsblc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2kxnpfeal.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txxzihuf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cbtktbap.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fnxamsli.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ajhiddbh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mznxlzdb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqirlxwx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2grniepep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vszstjxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qyjtrzwi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fcbldmee.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2earhxrwj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dcfyphfk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wvnrswuj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2urgtsbce.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qnhtwooi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ltcczoyu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dhmcbbkv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2mihoiofy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2juabjjde.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wbisvpum.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2tiymqtld.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nxyppklv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2urhfeqpy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mrdfjvfr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mgnebdkg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lzkpnshq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zzhpnxuy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2gypeuruq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2llzqvoog.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ashpjdoo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jzbianzo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2scesfqrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npnbpcse.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcsmyred.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mdlofgzm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dvhbsfmg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azlfoqyg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utpwevzu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lfeonaqi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edowyuqz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jmldjskw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekdhhfis.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfotkbco.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxjnvzsj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xexlwasi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjjcxbut.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nsgopkdb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lvbcctmz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tolisljr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pshrxuqv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ssymjatu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cesiytdx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bautmkai.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2msuwbiql.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xurvdeqv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ixdbtzzr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2qilcpiqu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xrldrihc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fasnltfa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2izidnxte.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pvbjwejs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ketxrkgx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dtxtqxou.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ejgshzdz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zkipcaql.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2uyijvytw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vijvblzl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzvpmlqy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qltoucmr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2byrfagsx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jhnxlhwd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2noptgpwu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kbdkgbzb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mcrgunih.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2dpanoipo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jovhzkvp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktejcdhy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eoqghfsz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fgciaxdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2puxmbmnl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odpchteb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ouwlupuo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cslhonwj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwhympzb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrnnpvdg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dbtjfkmi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qmjcjllu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fnbonsvb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lsxpdsar.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fzhoqpmx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rwsywmrh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zoazvsrv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2uqxvryak.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kqsqzgyi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2axmnpxry.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gvvgfagk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hegclthi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2exuvdxud.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ytjelryn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2feajuuta.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qkvqmwaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aczwkqkn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ogzapjnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmsfijcy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qmxorfbj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vseprfpp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kghqkltp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ljpghwni.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tnovadsl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hauummkm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2yzxqdxvr.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2duezdzcu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pqovmwnl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2daaskbhs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2azmlljij.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdjkzcay.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hgjlwfcw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgylcsks.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mmnbyklt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2aceuyfde.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wvpnjgra.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2thgmlorm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2xyisaart.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2twckljqc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sogvbttl.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ihlcjdty.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2madvdfph.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ejfbybql.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fvujejcu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zztwaupa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sfdnxkes.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gabnsnzg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ernbuxmu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2udzzbmru.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbcbalgs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbjkober.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tocbqawg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ccxdqntt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tihauxuu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vrfvfmws.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pxhkakgv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2coifhvfd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lirlzdeh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oktviihn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nehqqxuj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jukugyoe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2towrrybh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xtqsowcu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytceigxr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kohmoved.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2esqbfudo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vivcmhyn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dpjfaznw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2duqbpgwu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2shgenscv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2cesfiesh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2mucvyomi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2vdzukuwk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mmxewkte.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jyduplrz.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2kaiyjjpa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2isycnuge.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ckbulxbw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2siezpxpp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2xmnfesoh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ekzaycqd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvjfbb.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2byfzpewh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2kzsgyoyq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fujycncq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipvlwyrb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqgalpls.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2scyxjuma.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wqkvveri.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrzgzamo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2bxbnluyk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ikvzdzbh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2giwcqmmo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zelnnvby.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2csqwrpum.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2pwjsrgpy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2awmyiepj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2giwiytnp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zcrsetua.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2saemykbk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cwfpkekb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pcelfdrv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mrkxittx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2dpncsqfu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ywnkqool.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2faeibkdy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zlzumaaq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tjzgzhlr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2itsccphx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2tplmlbyv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2hoqkuxbm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xozfvtqp.html


<!-- 参考信息 -->