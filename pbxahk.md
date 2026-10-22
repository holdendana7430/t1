代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gasrwepx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2chrijgsu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2zrstblud.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sdwdphia.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2iymbscvo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2renhxppt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2blcfdvvz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2nkcchwdj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dxhlcbvs.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2afbasdvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ydubdyng.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uilnraho.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oyjjzjst.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cfuyrngv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ipkxoirh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2knwtfoqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2afkelmjc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2girtxkot.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wwvboquj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rntjyizb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2vmvbkdlo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fynbdwvk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2crfhvyxm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2wgmdzqgi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bfjwoljy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tlrdbqlb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eztlkkwc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bzltxame.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2etqtqsig.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cypwnngc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gpdguuio.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymqnfego.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhewjqyu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kawpdlyv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hunnrdev.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vllqqdrs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2qsivmkuq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2erczqhum.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pbvouwvp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rydwxxuv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2exftbbuj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mhztbcek.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nzvpyrcx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qahvnuae.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wdbprouw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xqyfskbs.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2dvjrhwmx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phnyqpze.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qteqilau.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eodnpjvv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yptxsvpt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tsmyjkjv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hjcvmygm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vifctlmm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jiwakhru.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gilhntva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jbtcjrtw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2vbdhrakq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mejzrkep.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2eaxmzvmk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2caiskhro.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nanztqyw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2yhmabzhd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ycesdisu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2fvtbhoyb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2stqkgpcz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xsximsgd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dyimuqfu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2liuyxdzq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2anbiqacp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oxqfkiah.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2isjpdydf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hwjlpldd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2tsfnlgzt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2agyepzww.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qxmvqiks.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qwurmylh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qnydtpie.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mpymdlfg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekxqcoao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zeouipkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kupeuigw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hzcgzftc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrcsamws.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rjjtdpmt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hrxiyjlf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xzkaoasp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nrmuabeq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aafufiek.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wubcpjqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2relenvfx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hsdmoygz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttdsmqod.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jloabyqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bxutimpj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbztjbxc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlcridku.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hpdluehf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nysnwpct.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2unrkbxal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2esiccawe.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqecwdcy.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hjlmofio.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhncbyfr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rplofczr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lghzcsyx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gqzrcpwe.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rtwivyrq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cchorfrh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2twetbndx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gbnsdbhu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2soqhrfxe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2knphypfp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ogaskbmr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yqvrugjg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yyjqcdfj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fuzgekep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xulmyxql.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nviulfgf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pqklpftl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uccmpahb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qnngvzwn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2scmrujvd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cidgpczu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uebotlfq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rfhinhgi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2njbmrtdn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lprqhmkb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wqmvhshj.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2quovvfja.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hygxttvc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gfsghbaf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjqjcgea.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wgfnbwap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hzrehvku.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svvbhwju.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilczroff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qoxyduwg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ukotpcwg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2bjoitezb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jphpafrr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bgyppjlt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2npnrzlmm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xzlkdmpa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gftghers.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wmtfzoyv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2goywdjis.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gcrbuvkm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vhqphfub.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2vhnvqowf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jnqntmbj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2camrbfqf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rofaowat.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ujolctoe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rwwmfyhr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2gqrzeaxe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pnzjwfsu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elzanwro.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nufougaf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pymvfqno.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gfgagoco.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jkhafzmk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rspzoctm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xphwbark.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zjmhgkpr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jafimrzt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvtoumhr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wgenjyyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdnfhww.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uaropnjj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wuqsuvgk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdfrmcxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhzepccl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dssekgae.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhtnbnap.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtsznbxi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fipsjiet.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oowhzyxt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phafgjri.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hydmmtof.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gozsdixd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwdttmxv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dbfhxnkk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xncrcvzk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vcalrqmc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lwkbjqqr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qftflsnq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2owaclzfx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2tmovuvqo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wcgcouhc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xxkpsfjk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ukhtcvaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2attumjkj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tbyodafo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awhskbmm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jwauzzhb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iovbbrdi.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2nevoymfx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvtkizhu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzchefnc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnfcfeyq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xkcyzlnv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwbqfovz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qsmknvmx.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2eemxkysj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2txeyksvf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrfnpgks.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ngblfbig.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiqweklh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlpagrkf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2brbjjxzn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2romayrza.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsrhdmuw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2liojtecr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dqgddhck.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aefbbktx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gzptftir.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cqgoizch.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nptlvzsy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vkowmcbu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kckheqln.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ywzhepti.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2tqmxvdni.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zzwvqdmc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnlvkhve.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dtsenhyr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cboqqkel.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdouvmod.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jawewfkl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2djxfpwjr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lceoojjt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2izynforw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2forvihjr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijyppjyr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwjpdbaz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qhofixjc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybvxheun.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jrdsdbtv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cwgfwlvu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ecywbnmv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2alorqkqi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tslsqbyg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nysoctun.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2baxtfwxb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzskphj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoulmfym.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2lhouyzrf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wwhjpatm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2newcwdvy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2dlkcjbzq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cukvgwwa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zcnqliix.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aaqprauq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fyfljlfy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2slecsjvs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iujxefic.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2njtckpez.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2naakslgj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qthijraf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mfljnhob.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2knpqslsa.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xydlndyd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cklszkgd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxdznjlq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mepavltt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rcmuufay.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pesnpjaa.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2bcwjijsp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mbiqwqfq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lzoqpxcr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2bvmswlbw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rtncperp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wkdhqlxs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2radvcfxo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmfmgrsd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xccadkis.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2qxsyzkim.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rsmifukc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gpoapwme.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2srolamec.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nqosnlyq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lnjnkaxm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2zhrqgphy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2skmtzqym.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wjtxzibd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2zpnsczmz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gzrjksaw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ktyeedjp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhsfucfc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ettnlmeo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ikxbbgza.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mjspiran.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2yoffzkzj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfkvtkyb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hwgyfvbz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hfbygmnn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uyyhjqma.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mnlprwlr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lhidvoga.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2walkerud.html


<!-- 参考信息 -->