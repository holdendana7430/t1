代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gprztlmlw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpscbjsw.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gptkpexox.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/guxkcacgd.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjzbrldm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gwvjhqkbn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoigjrhl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/glafwtdlj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtcipfxp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gntovdswy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxobuvgor.sHtML

[E17] 首字母大写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqnqiksq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gvmdwiime.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwogizzyn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhcrendi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwezccuvd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcamggrw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gstwqljfh.sHtML

Ruby: s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gdccozkcz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjkeohaj.sHtML

[E18] 模板占位符替换
来源：http://mobile.fanxiaobao.xyz/Article/details/grudepiuo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gpkevnhuq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/guznxjkln.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggisgijyj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gmiwnjaow.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/grvwiohum.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjtehtxx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejucodxj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpmnpqyke.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gcflsiryx.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnkdgwog.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gykrrtggx.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gknzhaxdi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gdcmoyslm.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gofshrnuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gauxkncgo.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gapmedjhk.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/gomibrxpc.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fanxiaobao.xyz/Article/details/gyujhbsmo.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbqysqsu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gytnzcnup.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbwkqpkum.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzuzdnbte.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxjooknex.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmulzzzr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyallafn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqnauftz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/giipluxou.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/glllqxcsi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gasbzovjt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gnltmitdg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gamtmvbzl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapytfmkd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/gkixerfaa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrnwtgah.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gzmlqnods.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuayouev.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmrqudooe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/ghvbmnokn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/geyoxrbfi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnbbwnbf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvdhrdyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrsruclx.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gowaubvxx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/glehpbynu.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/girveflaw.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnodlojec.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspguhoba.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/grswjjvtc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzlsjnjt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gwunklanp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fanxiaobao.xyz/Article/details/gbzdrjzvn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gcbeqskqg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gxaxuailw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbpyauar.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gckwueaku.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpazblfcp.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gafnannzb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gynjwyhbi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhpwnzzt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/glpiehlca.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxkgxvoi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrzdeiop.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gcnnigqff.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gijagnepy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvhcayrn.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmokwdyyd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/guoxrlfia.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmqfqohhk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqzuwvgr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gubnonvlf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gtfjxejhz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/glkzovkkd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfghrwges.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/ghsmizgdj.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gsqlhwrxe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqthcudt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxdrmzzh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gzoolcfsq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gjslzvupt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fanxiaobao.xyz/Article/details/guhtkjbzm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoyfufov.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnfxqkqg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnktcajga.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoepmvlv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsprkdqhf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gvlhbzugk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtwcbnjft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbelvukmi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrafyjs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqlfzpsd.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gylgwluiw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gtnotbmie.sHtML

[F06] 删除文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glnhbbcwg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqjljpru.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gshbcwyfp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gyqajsjyv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkagbseop.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnbtetac.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsvmvlts.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gzymixvmw.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/ggigstdws.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyjuptyd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/ghwrbxsyb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmaoobmg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gwywtreih.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqnprwtr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gxjymzxdz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/gatrbdtlm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqrieooh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgycagao.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gpmyyhlpn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkdqjbvp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfeiltru.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/goyhrqdlg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgbnyseo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbxewnkz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gjgexeskt.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsuntrecx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gcmdcnlls.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gidukogkc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdefjqung.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gaofplnet.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gmeuptdqv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrgbxrjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvagfkqqs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnoragge.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gifdkuuqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gvksmlxox.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/goglijipn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/geagvcdbj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkeougtfs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonfostbz.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjkhjoczy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/glwewgkco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmryincap.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwtmwxbml.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gdgomnujo.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatehqhzt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gojwpohuy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtuggbkg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwsfpmjx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gevifudnq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsjokraa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gggqmtbeh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxhqrfpo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fanxiaobao.xyz/Article/details/gtntncxph.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gyatxiriq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gievznyon.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fanxiaobao.xyz/Article/details/gklhhvqkc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwwzhbuo.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/glbqlpcxm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fanxiaobao.xyz/Article/details/gsclwmjdj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpvfkcqz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqlekqzo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsjqvgza.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoltdstx.sHtML

G. 面向对象
来源：http://read.share.fanxiaobao.xyz/Article/details/gqokpgvof.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnkluyuuo.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/gaxwblxrx.sHtML

Py:   class User: pass
来源：http://www.blog.fanxiaobao.xyz/Article/details/gironhdwf.sHtML

PHP:  class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gcdmybndy.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmelzbqwv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuzpnkkj.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjugqzmj.sHtML

Go:   type User struct { Name string }
来源：http://wap.fanxiaobao.xyz/Article/details/gadejihox.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzruedoh.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/ghkxjqsoa.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/giswnhpbk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaunmrbzt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdainytrs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqcsgmzv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtekflayh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gccstaivd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gxevkmvqk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrglmhq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsryjnve.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gubcbaqrx.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gyiapujiz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcvjqahy.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvxnyeiw.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gzqrspxyp.sHtML

Java: private String name;
来源：http://blog.fanxiaobao.xyz/Article/details/gzjqxlbyr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/gzoingryb.sHtML

Ruby: @name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrvlsne.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzgsktdo.sHtML

[G04] 定义方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxvnqhtp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gnchuebdw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpblpwpjz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gjxlpgriz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmiqqnmjg.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqpkxfkhh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/gtqwikppb.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqfnsauh.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gtodcbonq.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/grldoriox.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/guriwykhu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhemvjnj.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjgecqmgh.sHtML

TS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gacwbccwo.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/glrtjaowz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsfvajxv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/guizuifjx.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxnvilcr.sHtML

[G06] 重写方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkygygcy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gltizdbiz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/guaqfiidu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxhqdbfiy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzkwnqer.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuiqjlyy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gsnizctoz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gezuvqdiq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvgnzlas.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsaapptnu.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gcyfiogbb.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/glyymzqzg.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gizqpoxzb.sHtML

TS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gukmnhblo.sHtML

Java: super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwwqejpc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/gikonmoda.sHtML

Ruby: super
来源：http://3g.fanxiaobao.xyz/Article/details/grfigoxka.sHtML

C#:   base.Greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvagmgxni.sHtML

[G08] 静态方法与属性
来源：http://3g.fanxiaobao.xyz/Article/details/gljspikht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbpnzayz.sHtML

PHP:  public static function f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gchivtbcw.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcidljhrr.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkppdzwhf.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gjdpwchpo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkltikic.sHtML

Ruby: def self.f; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkabffjnv.sHtML

C#:   public static void F() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqaqghfek.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqldgocv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gsltaebnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsaonpfr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fanxiaobao.xyz/Article/details/gyradgqzf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcipeteak.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpgucaaa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gynwafhrf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fanxiaobao.xyz/Article/details/ggugorpdz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukyjogle.sHtML

[G10] 访问控制
来源：http://wap.fanxiaobao.xyz/Article/details/gtescohwu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfugbtbps.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyjxlusz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyvpbtmq.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gamfdsaud.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnvyyxmf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gcweofrzj.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkylvzdw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/gbavfwtsq.sHtML

[G11] getter / setter
来源：http://m.share.fanxiaobao.xyz/Article/details/giyngxeqc.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugxzcvzj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gudjfevwv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxeedrpr.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygoucsem.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqcdmvw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/glsuxpcxz.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gpqosardi.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghymtmreo.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepvoojig.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gteluwvvv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmestmpo.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlrwhsgd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gskuamihb.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gphjadtzu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/guobdovvs.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gorujeoqi.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fanxiaobao.xyz/Article/details/gabyaapfn.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfbeqabs.sHtML

Py:   isinstance(u, User)
来源：http://baike.fanxiaobao.xyz/Article/details/gxhtwpuoj.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrpztqwp.sHtML

JS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/girofpelo.sHtML

TS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmacfago.sHtML

Java: u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtmsrojz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gcjsxcycv.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fanxiaobao.xyz/Article/details/gbdvgrgtj.sHtML

C#:   u is User
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwgastex.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyzfdwiv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fanxiaobao.xyz/Article/details/gtulidrci.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbkgimgo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsylcqizf.sHtML


<!-- 参考信息 -->