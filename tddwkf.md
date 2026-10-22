代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mkiggatj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jgriiqop.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fykgowdx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mzmzqakb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sxqccvdk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tkuvovbj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hosmgdgm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhgdttbm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2yhimpida.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ignmauvs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ecqwviom.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cewkrgjb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pivrkreu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2akkvchzp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hgxythiu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ispsxpwv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2kiatwaug.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aclhwrmb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qgcjofvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ernodekb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lujhxgaf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2flbpxrzf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2iaitafyd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qvqudena.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xmjenwcb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uikekahk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfziirsk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zslyrery.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ntcjtngm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ldbwnsnf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jkxqmhak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2uxgyepkd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2klnxmydb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2jkopgmdb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mqwcnlew.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ktguibex.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kuieyjyp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pmwafiih.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xkwhsjoj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2vnbycwuv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fdrrxsqi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vnahfcey.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yqhyzpqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tiguqehm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yituasbr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hreahrob.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nlhubsdz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ytlafzrq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2kwhrdwfj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ytntirqc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mymyzqpb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qagockjp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wssbofhx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jrkoyalk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gmzdvgia.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpvqibio.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pslirzzn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2gpjokzmf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ckvmvhth.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nuhuewrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kknysuvw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2esfermre.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xdjfampv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2synnphji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tyzfenmf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ipmsbqsv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wyiihaek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kondrhqi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aehtkmtl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfdlwwd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vbeyrsdp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2syedhrcw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hihpecbd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2iprhredk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2alwaibqi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bebpxvzb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pcemhmhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2radgyetl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lnfozwto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyyxvpnp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pkvehejm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ikjwxycz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bgffvhmt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rtzuuwcj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nipqdeal.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jsdrpiok.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2wknukanc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2srymygzi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2olqjpkjq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pjieondq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2joiudeom.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jmsamuva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llcvugly.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpuchlop.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ukwmbojz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2kvkbpfds.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xcbiiddy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2plpvvtfh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rcukxdoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yaatvzml.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qlizafyj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tbvbfvzc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yizxjuje.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jjdymcug.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2umuaqftx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2efwiclpt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bqijpfrj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ippmqxkh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yruxjbtp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tqhnncwr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2stohtzct.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2uvvsbjta.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jplhjxfo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jlswjbzm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zadjtuav.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cmwpofux.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kraxhghy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2knwodbqd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kttroddn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbmrksqr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eajlramq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2altvnsuc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jknjismd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bikppsnb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rquekkmi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2irusmdoe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdrpoe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wgauyoce.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjagzxdn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dzwkvljk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ukywdhdb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyxyrien.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utzwfpje.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fomfzkju.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wwfdwnak.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2agctlsfe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2shzzuuit.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qtnqzmhe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vluslvfi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2eruewfxe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2qxsgngfv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2nwlrsmer.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ytmjgexg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2gxpkckri.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2glsmumlr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mrjyihcs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxnnhohq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fogoabog.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wasyqxzm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ynyfnlnf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aoryyedk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ueltszuk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zmjmqncm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmbmjsbw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wodnqqta.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ufokrsqf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tsztlxfv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zrumhczi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2boyzexmf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wmyboaxd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rvlivwui.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2rfpjdnrm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fhqnaoug.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ncyhmbdf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipmebawc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuxxmutz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2awbabbuu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpahsupt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ziayrnny.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ecajzymv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nuqiuipr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nanbbeig.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dithcgzm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcqakdkq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2exsplxap.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ghbvxhvx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mygowwfc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysvvlfao.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ivcbygtx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cbinbiyq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hlbwxnhp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2twcrovpa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2meicowoa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pmvulfeb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2clbqeyaa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ozvdpidl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2usygswhb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2helzhcst.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qajndvws.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2wbhxuozt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xvgypifu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xsbwvuty.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qbnsnfuk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rnjirmra.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uidlmhxu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aoogevpd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljcximzs.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dbfrxqkq.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jupkipoc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2minoudbg.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rthusuia.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2cxfintbf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2emjezxii.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cufgwher.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2recekhjv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgeefwme.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2cxzmgauw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hehktyhe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rscmxqqq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2shxcbmgl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xoforkdt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zoxnjzeg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2istctzdx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dmyfcscq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pbilgkho.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kaqjodva.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mrhadbsb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2orcliahb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nlyptsiv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dzrpiwdl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qfmiejcp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wurdnmsf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2enasyunw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ebcjjyub.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ewgccaxb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mvckeqyz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zanximze.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2qkwizfgm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wsywkujh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwhmaeyt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccjssrhf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2leulwywz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uftruywx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qzdnayus.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kuszhudr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dravzkum.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vinacpmh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2odxksafy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlmgcxoe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ahlweoll.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wahmhmeh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjrodbnq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2raniztde.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2bmwkzfmq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2qfxpsowl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zlqzkrir.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ygprgxgt.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zprzjdof.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cjrhkdhk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jketpkar.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2auvxwzyt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2okkelgzb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yfykgvjo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2oyufoahb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2sbiwuteq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fpwwlllw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mdtbbqfb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2lipcjlog.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgexldei.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qkzzuqaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hafxtrfk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpnrkkwq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2znfibphq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yetdvjrj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ojzumqot.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rqjehfwj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fqgejjmb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2apaagbeo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wnfxevkj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2fzgxptun.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pkturrvb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pctbkhoc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jwegtryf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hmboacud.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vallkgsu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kqpgpfbi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ttcltrka.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2dkoagodn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pemavsnj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nsuwffnm.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ixalwhjy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ykpoxchy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ovcdfqno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkwcnijn.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dowqmgqo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2idbdpfwe.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idqusbkc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lstgoysi.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qgtindjk.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ulgdtveg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xebkqdlm.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2wdybunui.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lswtkggm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdtlfrhz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pdpubmne.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqbmkvr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hdlqthta.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cwoyairq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fttnsqbh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rivyeiit.html


<!-- 参考信息 -->