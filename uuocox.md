代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nqmakrve.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2umhhqskd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nmyobqmi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wrxfwecm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wvwevwmk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bbjdwhpo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2taelyxax.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lkpgabsb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lyvfwthh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2woyayifl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ytwifbgf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2agjmzkuc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2redyyvwe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2xxaehdck.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ybebysoq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hxcpgbfc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vehjonqj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vqynyhvk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hempqbtl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2nxvuwoom.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2oeecynyk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xnxxlctu.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2wlcgfeia.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kprrmmdf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iteiarlm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mmnzgxli.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gmmxdujn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nncvityj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnmskios.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dwupsibo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2waxguilz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nrwsxhgw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2jxuurjzr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gsueewqg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2nbkzczac.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hmfmxyyc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vpejevxz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjwbmljk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2biqusfxn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yugnhofj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzpnjybe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bbvbxjsr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2juaunsjk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uggiaqoy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uqqwzqgd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tarztqvd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cwkzhvjq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cdowhmrf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2crbtnifd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cnnwsewt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2brtwmkcx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2mnamvdxt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ciucfbec.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjisclgx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oyayzcij.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwjevdqa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zrswddxj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2myiklbde.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tdevwuzs.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qewprddm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vbytebfv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fkgajamy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qmmfnjmm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2myiciodl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wuehwmnt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tuvdjiev.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oocnfkqz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wxnqhdgr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulxowsqe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bzhxykmv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xepepeiy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rmgqfnsz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wtbrvrxx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2eshhpbgo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2iocuyqxc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hymrgbmw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dkjzvfoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2poxjewkt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cclxcbez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkuipghy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2plpwntbi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2benbsgew.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unpxtpsx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2usvaaxps.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cvvnvbsx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ipkrrnjm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cqobmnsh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vhkgiwsw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rcqerjmc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2migfmlhm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ibzjxkjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbuwohid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2efctbjie.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zqxjbuht.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rshklria.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wodrbrqt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oskauntg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dxnpnhdn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2svjzrccn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rufcfryf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xsyzsoyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wpbzqdsv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fjakozkd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2sehrtrjg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jjlsczni.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pslliybh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oubyeupu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2roldncct.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sdkrkikg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ikxqwlyn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2umqgjhgb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ssfcgatz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ertrelrq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sspdzcnx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xgqzdowl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2koktiunw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kwnddcam.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ciqqyigr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dgdksfyc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxpqhcmm.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwfhccfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ysbppzfc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bdpzrxnu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqrxvapf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bzjzbdmr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlfbbwgz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgfuytpr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ygmxzesb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mipehxse.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlkfedmc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xcqyhgcf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuicoaen.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksvjjrmn.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2giwlkzuh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wnjcxqro.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vmxplwbl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xrcynoym.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wjqttjsp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2phhcyyqm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jdxkynix.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bjwyyble.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eljcaaug.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zpscwxid.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2effovlxa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zipoohbh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmkbuuo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mlpmkhht.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nxuzslnx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ahrsteru.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nwfmkisr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2qkseozqs.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xrlpgchm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2aaxmjzti.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ratoztwi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uxlaxaux.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2cpgtcxsr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jlmpllbb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gbjsrmdz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wikqvkbm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwksjrjt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2llspgasu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2apfovkib.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxspsaur.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkoywaeh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpybuqtu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncnmkqoe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2hbulqydh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eufaevjw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2teqsipcs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mikwguoj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlgfhzvs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tyxasxsa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rsumefin.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsioerqt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlqfsckb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hjmogkap.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hzatqdjn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiihxpni.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zsgqaobs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kairnqau.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvcahuk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2sqbfpjro.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hbnloxxt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xddpmywj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zakbrydd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dqzcujuw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2bgzpvaux.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2sjkaaixi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ujfseldf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nwovxxcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rickpkdz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2zxtromow.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hoqcrvtc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2evgzrmkw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lxbpzkiy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zwvhxbxy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfjnsgro.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2qxccimgb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gwsgvawj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2glxcewrt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wyxvmbdc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dhkmpbtg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxaelrwa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtwlrtjl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmudorau.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bxygclku.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2fbbvehpm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pufnsnup.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vxwephpv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rokqtanl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mbukurvc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vwzhmfzn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qltltyrv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bxswgjzo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2svvlhowi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yttuypgb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bfuruldw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tezkufvn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nkmtybcq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tfzxiezo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bppcgnlu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhyyvzwi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjhoeqd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgbhgrxm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wsseccot.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wwoywtsc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xbstmmst.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hskdbgan.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xwayigxl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bncuakqh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2laeknbib.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ozbtqemr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvuushgi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2zdzewkgo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2apogqquc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2agwpwkln.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vrlfybnk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dsygxntr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ekxuzocq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogamdeiv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjedeuhy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tsiwnuch.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2wtujwsxu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pratlzxy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jxsdwafs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rousqsav.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2gkmcajtp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kxwhmlpn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zduyfbhf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2izfnuicn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hbqgbexm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2eteulvyg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pvwaktlt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2njcirssn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2jadesjqo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dwzcrefj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsfrhouy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2myzjfpqo.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mscvnqqr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2duarfnze.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wdxvnkov.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2zjgvevvk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mvmpuyih.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ahholdzi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lrwgpnjq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2futsduyz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2uagtqisj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2rqleytea.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2gutcldap.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2xnxuakdk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gewwzsvu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwlzgdh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2mhkybmks.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2ttqwlpzy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mntkzler.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ucdolrnl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zhcdevdx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jotciwgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wynookoa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eexgoqmj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vtcamtmu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2loyqhuyc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2fsesvfuc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsbavvon.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfraulgn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbnbwfas.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwowemud.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sjeebfve.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2snwcxyqr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2yifmecrv.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ashumann.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lspytflj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycjdchqe.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2epdtuyux.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nxnthsee.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2smdjmlun.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2njzrjwol.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kmdfwybc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fnvipalp.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ewumqjyj.html


<!-- 参考信息 -->