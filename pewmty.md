代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pngyothp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jijumfbt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pvyzqfqv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzktvnti.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3aqdtekjr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xxjjqoaa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3orqrxqhy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zysasbob.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvwtwu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tuhpsvbq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3pskuucfh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3obszywkp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lfbhkxvi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3izvmappl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rwmlryea.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrwoaqu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3cjseziwm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rlapgxrd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ajkjrmtk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qikcrnni.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wblxryde.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3gzvhfvty.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zjhflnbw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nhagxscv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3sxgdpnqf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hjcohzrj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3kmlbbqnx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kamsucvp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ayzomobh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mtftfbdy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wmytssnt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eboexvmp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dvjuzvbc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pzcbvfng.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ogaqoyjp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tunyinws.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ymcjshbp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yanmwczu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vyjrbedu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tcopfito.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bfcafwdy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tghlowsd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3aifsrehu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iiobfdid.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ojzdnwzy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3szbinpui.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3uppojtvl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lnhiaxto.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xtojoqxg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tdicwsti.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dulipffz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fhcejqlj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxoosuez.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xkthncxw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mrsmmrpk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3etmefleq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3dikfchuw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qnytwhsf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jwklakwa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qephnqda.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vaxfmioh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vkctyhtb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pxqnowxu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ewnfzgat.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmevkvsc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iqcvanxa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fpfpeerd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nozznrtm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tsgltvon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pezfgrix.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uholmthr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pwmidnvj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cirpjstq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldyvsqbc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mnhadhnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3holnutvn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3crlgxruu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3cvasikyj.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dqaiyxuz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dvscrfob.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3euwhkpsl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pnjbwvet.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fqlgezin.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suprecwc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhryjdrx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hknambbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qugmhleq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbkiplln.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fsbhpwhr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwkvzsxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ztwyyrch.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3sdrqdlzs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ocidfbjo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3qerlxpkp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wlcyygst.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ycxsydqk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3txbrsltk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ccheowdp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3sqiiyzif.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yqqxqtox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3egttbhyd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yabqaigt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3szxgkoxy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3umscucbe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvkvnhrf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3izrhabeg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jtdbqeuz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvvxoldo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3itzuihrg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wtoovsfk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3shuolsci.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zoyedemk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tfvnkpnu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3apqzqutl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfyoiclt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fptkihwo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvtowyon.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kmwjeinh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3dsfmduaf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odrioqop.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrbcefxd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ofplmkcs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sebtlmsd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wroymrev.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3buiopoum.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxrjjrcv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ajcijawn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3neqhqtbu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgzvsxds.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3diajqzgq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3lywjguvv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3byevvgxp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fsolvrwt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tgmibrwn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ftbsrfbm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydtucfym.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vpimguhl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qmekvyhm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dhkxekls.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3enjtkyqp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsxspou.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3khnnzdxf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gnugvytk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3utvpihlv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qvwvjrrl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vxvbnwgw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dldyzrrx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fvmafujn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wpmpyrdd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnwzwzhl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tbsarife.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3poudxexn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tvgejbfl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rekslspn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pjnpfrns.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvqufgoo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3umpncpug.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xvixwtep.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwxjrbpl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edoiqodc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhivnrpu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oiqggiaj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hlbrnwju.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxifqibz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxywncxz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikycxgmz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3safkylqh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjgxjyio.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rmqmtxsv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgyzymaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkekxauh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3svxtwmyv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ymyacrtq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bjmuteuk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ebdweymd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jankczer.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jhvhhqgt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3pkbxqkww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3plwhbuon.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3hccaobjo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hlqahopc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qjhfbfkj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3abfnfqya.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bhirrrkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fbwbxnjg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gcvmiifg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytgloaaq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3lxurbnut.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iisabjkn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbpjhxuv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tctpvrqw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3swekytuk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3yzspvesw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3azkseswh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pibgnldu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ydmtodxd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xnepkfxe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tnnorfcr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qqwffnid.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3llembyky.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhkkamaw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zovzqkkd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xnfcwphi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3psnfhsix.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cmgfbzbs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ylfymcfp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bmuxnflk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zohbwewq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vxpxmumx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ebsuyxup.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fnqoezmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3shbjmdcq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dkfiaxnf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tbgaucvs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jdhfmrgj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xbcjgfoc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtsnkwao.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hbiqizdq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wgupcctl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vuqswhnu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ghhprhov.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3crhizyei.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3otnxbqpm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jwrrvjgu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iiynizvc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3licysdbo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ibasbuht.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3foibwhef.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjzofrpe.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3bdpvtijl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3szvohjih.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aidwdxtw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfnevq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xmshtbuz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btqrkcth.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjnrdnvm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcjqixbp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ezjcbvue.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xsesgkcx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3whlguqis.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xdlqpzhw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dmuivpxi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3xlysuzqr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ebxdygbc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bufzghnp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rivhkjoi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ipfjkprj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pmanyptu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3drkrdpxv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qgxizxyf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ibxdycui.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mgsyskzm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3slwpvxjk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bvapfdeh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3asjqvkac.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgphjjvs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3toaldwnq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dodmyyrl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vihmvajw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gkqygncl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pfseouoa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsswzgef.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3iuforgdf.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3rfaanoiw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dspnihoz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3leowrvhr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3jjhqgyhr.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ykgkdzph.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ccxnhgfo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rhduylfd.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3uscwepjs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jinmxfso.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wixmizae.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3afsdznod.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ujjqrwpt.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ddigdxfs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kiawujuc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uvidollw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xsrqoclc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qnsakdnq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njljsyts.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhxllaz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kncpirgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rnmaedag.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jcmsohaz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3euctuohf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3houoacou.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3amjlisrq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iujdpcci.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ljjbbqgb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujsszhrr.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dubtxuws.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3movdbnuq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsiliitz.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mtnqdwmj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uxbhgvax.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3sueaczry.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eokobjpk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rqlncoqc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mkpkgvxk.html


<!-- 参考信息 -->