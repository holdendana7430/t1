代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2efybcgnj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ajmeqcmf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ereyxxtu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2cxwrgkrd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gorbwpdc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ewpehyum.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2utbfmatd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2orxfuplp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mxnhyoqo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nltwdguy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tqtqepmu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fjfnuiyu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ypuqvpif.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lmywbkym.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2tmuonxdv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ifzrpcni.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2akzponwh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2awbgzwkw.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2uizvhbcm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sglgtbam.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fepxspah.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ckrrdbsu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jcprohzj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2frjzghbg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzsreb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2efqabizq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ynafydxb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2abrajdoz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iaeuruch.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wppujyfm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djtwwqdj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mzejlegn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fnzmpmpt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uqjzwzko.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kiotneuq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ndhmqyvq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qxosjnrn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mhbjxdcp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2xavpqgax.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dxyrzwyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrxophr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2porvyiqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rzadrboy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cnrootnd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zeidpidn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zirtgfxr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hinotyox.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iymuogvg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vfcwqbrt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dlivwwpc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iesisaon.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2bwpldyen.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wjjslycm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gwegiklq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ccpjiitl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2hnujwhnj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nwxcqibi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzuikvpk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2aluldgbe.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhuxssoa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lxztyirm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ygsqblfr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgdltuil.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2fwfmyqwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zflgyfky.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aiwzfmpy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xzqigxry.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cxijkket.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bldsyppe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2jfhmxkkk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fdgzhlcd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zszqxxdl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gmkgxhrb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpnbgnf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pclczlkf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jrbadvvz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lsdsugmc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zihotmga.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ijdabmwt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sogzxfsy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ugedbsrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thbyvcms.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eycwabiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifdidten.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2swgabjrp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pekclpkk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2btilpvyw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lgiygkxw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jydpuiji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uipfapgu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2anixfggp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hvferigy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bednqjkh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zjrepsnp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dxhgfoju.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fcdflncu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gfldsryz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wambtafo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kujiakey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2iyipppjy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pskbxiad.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlrdadns.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hcaofbdl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eiiaxeqg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2znejitmd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jdxmstul.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2avktlget.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zhytvaez.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2weqbojqn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2daxjfaum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udiapftv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dnfhjhva.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gcqhblmx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eztfqsjy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ikrerwyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2pwkpkniz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rqxmkojv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pkpjlifz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2pmyhxbdh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2otwjhflm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zkwguzsj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2faywfarz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rshkyfjk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqdebvon.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2negyutfh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2neuqmntg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rmglffna.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvvyrdnz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfnlyqun.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgnjbwul.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adphzxgr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ghektqwi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdwhhbom.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dovcabzt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brpcqozf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtavjioi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waveqtkq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpovtvvw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2hovevnza.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wxamwpjk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iqxaxfqz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pjqfubkn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cbltysfj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zeavahno.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yicdojmu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbvlnyt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pkuutgzf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wlggtyjm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfygnfon.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwkkvwsq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2idpubffh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jjqnbatz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqczpa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tollayoi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cjvxqfjr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rizbdtxd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qsuubgez.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jdibbsmo.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xmumfpeh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kjzcjxav.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2yjittskb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rpigcplf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jawqmqff.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orjrislg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2taaxzmpv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hymspxdh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwuhesro.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ujumkspt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdlsuhqd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xzithwpc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2zdahdfhv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phusaxze.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkwxzeph.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rglaozre.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zugmnxtw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dvqetlzy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tzakzngc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuuvnvzt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsgbarne.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqmnnvd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uvrthokt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vnxqajej.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gkdyjzua.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zhjbkjkm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2lladksju.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hrsysswz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jttqixvn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ophueqjt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2mkrsdnjr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2aojrwmnw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lqkdlcps.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2weqnzgvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnamsjwr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ajnlnasq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vvygupdm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pdjlxkda.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kvsiaybk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wzhubbxe.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygazqdmd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cygybptd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2syacjvap.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wcobzbhw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqhxszas.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdlfwmom.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2apmjynbo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2hqeuksty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbbgguhu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vcbyoejf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fiulapdk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hrlwxgbj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2htvvvqaj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2obqtbkaw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aiovnmem.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ebwtyajc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ytfmkdkh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lazhzxlb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2swyctdwt.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jusuymln.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hfvjeeoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lvfrnzxp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tvubfkyx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ndoknzpr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xxzlgrnc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pgwcltvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xqceaijp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2czdivzrw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohanhmdx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2phjrqxhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vbhbhoga.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hlepkuiu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2qolspdpx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2amtiyzcn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2enplzzgs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wukcfour.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvtgcota.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvtnkkfi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ztqhieoa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mrfrjnnj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ufwsdtvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oieksxxf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mjzuqrjg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2sjkwgllj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zalvnhvx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hncghzsi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2umqohwsf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gysqntda.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwyyre.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qqbbaxln.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rtctlkqd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2spvnprce.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2jvmsckja.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xvqxlksy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sqjuykcl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aeauunwb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hlijnkxp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iiqtrsag.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xjqfzdmr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lssdrsxk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zeyowffw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2aedjvked.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqnpwfmu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nifpluoe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2siwyzwmf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgxleiyo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wbyrabxt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjeodpva.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2aaadubcn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ouebjboa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lzmbykjp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2yfkiymqk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pfjkzowx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2swkydbam.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtdawtac.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwkxuyf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fxzpkhwi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ogihpbkl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2oqltubmc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2qyhgrdjx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2twkisuhe.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qucbecck.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dplnswqm.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ssnkxceb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2lfnrqihv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mcubhate.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2neijjydm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2adlenpva.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2omfznjwl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgtiqiaz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoigmrvl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rlhrxnbk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zhskdvsl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2icwtvzzt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2phwvjpna.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cdyqueiz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oarleiom.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ycxujkwb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqwmjgkg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrhsojxg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlhglilf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xysbpdqi.html


<!-- 参考信息 -->