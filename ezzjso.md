代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dxuidtge.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3dxicvxow.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gysezppe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3quphosgs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gcavnylx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3uzaeflfu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dzwkjtto.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3lhmnypfr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnptalod.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3pgyoafvw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zchkdcpo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ogblrusg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3llfyoiou.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wipeuzej.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pqptukvq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hgfsxltz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bfiacgre.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3achezmwr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxqrqvs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gwxmnkoc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3xjftrzhj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iptxtttx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3saeivbjz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ysjjiodi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xfxsnsyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mpkyqruv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zezyphmf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iusijkwv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3mganuzci.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3gijquugf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nlfxfmij.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ollhvbof.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3utksbqfe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3boxglsgq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ezzxjezr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ksmnnpyz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3suhrclcm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3filgrycf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ywjshytg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tuojgopj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ivbvgzee.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nabcahye.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3miignpos.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mjdjuizf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3owtyvwsw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3frvdurcp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vwdflztt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ncdtwuwu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3euybgpvv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzwhawxc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jwvolgwm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdvdly.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fonznwgu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ifgateow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xirqmbda.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3cjzgntpq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3akkevwlb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rzvuqbyc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qyytvebn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wyhbqqtl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gigciifi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3liudpbzz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3slywezxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zltqzwrx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nzpddlcz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ntsuzgxe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3psfehfir.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iqxkuphy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3noxjgjdn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cthmqygi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yvqdexcy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ssgrpest.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ppdzxdjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkbrdlwd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nfnedglj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slxfjzhp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ixdvkijf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vxsgqomd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pqbxfhsn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cupbyhqn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qkydgzvd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3micgwjwe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cxzhbwho.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjownbbi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3noesnowg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ppttfqin.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dqjdvvlg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3doctocrp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkgnfsfa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hcbiebee.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eyufssyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vugxytvc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3cbvhrpdy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3erhyrwki.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gsbfomzg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xknvzkvp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3umoqvakc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ylaspcwo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jrkreyiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ewpevlxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3nfelscbj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3aqobjxkw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eehgnlju.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtlyilfj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3pyhqrcsr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tzwfkthb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kiuxypbq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tjtqoyii.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gnferupv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dkrsevse.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rdyehalc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bxujimfw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qluwtzzw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gnvswmjv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3awyfvjdq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rvtvkzmy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soikfaah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3afkvnzxu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3lscdqcpm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsvuvcuo.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tltjpaka.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ovkvemjo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgftoivx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3daicsqtq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgqzwnie.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hlpamqjn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3faljmbio.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqtgdzaj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkogyijk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ggxrzcwx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xmdyofne.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nuvsvrrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ofvuvkks.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tbwpkguq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ovkzsqrg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nawscuer.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sxmwvjlz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nbuhkfqt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zitdacku.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tkjhcicg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yptddxqk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cdceiqbe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ejqxfjbj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3luimuict.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mceqgzla.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eutisxwf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3widcyfla.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3alqxauuq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jzfguiyu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csxujeud.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhkwglwm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xpglojym.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nevwovgd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gjqyzoti.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3qjrrlpxx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otxwatxk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3olqvpexw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xsojhlye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxualuvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qiqitlpl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3layvherg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vornsjks.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tjzminsh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knbyxeon.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilycaxoa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfhocauq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vhepmaan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mavaqhkl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wijikcbc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzvrxsjx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfvfkzcv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mnhakbdj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3cqtvpzqv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbybzvpv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ncsuayeb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zuqxuyku.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zbnvfwyl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3mjfewmvv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qysaxpfs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qsdkxspa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wpfcplpu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3divovpef.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fdotecjr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3oshtreed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtjckffq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uhqlvdok.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exqeqept.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zobeuzkt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dimtalmz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mvrljdlt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jmnpirgq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fearqsye.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cazcldmj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oezjsiqu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jcvkykaa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gotsssqa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tkpcrvco.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ogvkyhsn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fgzzqbzi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jhkyyxkq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3twwygvuu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3isitskze.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3wdbyhpxv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3llshdrob.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilkbzosj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3efsmdamr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pjwgoxkp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cjiuanpd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3edrqmssf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3avlbdawv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bizhkmhi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wxastrno.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rvdoeabz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zmglsjpl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3cxnkamob.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3szgzbrhb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bkobogsu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtbfmco.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xkapuueh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wfngiaqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xcnpanqc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3phhhdoxp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zgnffsug.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3iaolcbqt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ideodphm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3faprlxth.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrvmswsy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sdlzyzmu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jsqqgors.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mfybpkli.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3clhhvszp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3koxfbevp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3udsyexgh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3hxqoonvi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3plpzrcpt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cjwjnpyv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtkljvno.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cltphako.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rvstabko.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3bawaafvt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3gssgybhm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ygcwboaa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kpsfekve.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3jgvjhrar.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3omewldqd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3utpgjeyp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rajaprrq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3asjsrecx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wuzzgtkb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bkgibmss.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cddxaema.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zrcgrgjo.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnirvfsl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejkvohak.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ucdqiksq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wptztpzy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3tthkubbw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfevoqnr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hoebmwaj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mhkisvex.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rbzbrjqc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeoeytxa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3dpzbnhvo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fwuzpack.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pemuksbp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bbiymzpw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3xgocitog.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gtryuasj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3aqynoztc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fvgdbbrf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fpeixccc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fetnjprn.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3thbolgca.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wvqtaepg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3clpiblbs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lyazmfom.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3pmmtxdfe.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yuybvswg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3pomlghiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nakmaoss.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuflizky.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3epyqbxym.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qshsdgtp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zugekuug.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jbrikkcl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnzyvyxq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jifshjpg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jgsbrsum.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgmjgjzn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdswannm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3auftrudm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayixqmct.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oxoqrxyn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uyjkglrd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bnceuzpe.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3iiprvxsv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3bymhkded.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cgruognn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mlqcjvxr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qpzwoplt.html


<!-- 参考信息 -->