代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/ghhlogukl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gwlvgqwuy.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gwhtsgizb.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gagkkkxvn.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gzxaszbto.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gfagvdqlw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gldmhejiq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gkpzkqjme.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/guqblxwdo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/grumxrnpy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gddbatgnv.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gpysaqeru.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gkaayxphw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gvbdbqtsk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfkbttdc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gwjkheqpo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gtiqqdaoo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gzxrbvvlk.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/grxoorqzc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gaqqopfvr.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gvhmazvvu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gtbyzjgzl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gokxhhihk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghtdftgwf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gosgowkut.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkqnzrbge.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gbyfshpfw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gxqayjnsi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/ghurxpwll.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/geiskhjuv.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gchumcnhf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/guzixazst.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gvexdetbu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gpmydsrmq.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gajuzxnzp.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/grwufxabt.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gmaxfpjqp.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gfyqifnvm.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gkrndwmjq.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gyaucvruv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/goxtvehiv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gbadkigil.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gwygglufy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gzdbnjypg.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/ggkiyjxvg.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gliitxvpu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gbvlgwiga.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/guybhvmtb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gmiczppym.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gzpzcoekg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzymytnvt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gurkhhovq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gsabczcit.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gftkhnmcn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghswsrzph.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gfdgdshxa.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/grjhyzjhu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtnezaruq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghazrczed.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gwvzbhhlh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/garjgafuv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gmknzaivt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gtxqdrqjs.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnlxwvevz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gygtbcqxi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gayucdbdy.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gveiqfzfi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvsptqgym.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gkvrcgatg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gtulfvvwp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gelaafnxa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gbidgywuh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gykueenvp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdhiidpyx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gbhavswxw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gewewtbxv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmeyxfhgm.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/ghmavvesr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/girupbynp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gcvgfavfb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gkehljzby.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gsenlynzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gisluvald.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gbxauppco.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/glyxhxcvm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gamcqxkgy.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gbetqejxe.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/giayupjwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ggjvszztq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ggvyijvgw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqctzpmyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gmqcrxqsp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gnhydapyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gctnlanpk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmlsyfdan.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gktbigkhr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gbcicemtu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gpfiynmbt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gdtipwofb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gtmjiwpuj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gktynkgdl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gzzeosxal.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gfxeepwzw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/ghgwbvwth.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gtmsotvjv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gdzcnfolv.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/glhtgkkda.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdbtzxjla.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtvokorub.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guhqyjcsi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/ghrzpjnwu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghctymksv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghiyzemos.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/guveibdic.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjhbwnqox.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/geaqqaoqu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gecnxuecv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkndhmsjb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkvsbfiet.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfkuqjzbk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjbkiswbh.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjpldigmh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gzygmfkul.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gesbbzdpv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gsblwimec.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/grecpdfgu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gktfpkqum.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gydemhsua.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gjjqbezts.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gdteqvjls.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gfpfdlcoo.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gpobmglnv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdupjiap.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gmhbapcrc.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gjcoyilqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gtfdklsvh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gfbowaxal.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gfydqplgq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzzfzrrkj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnqlijkgl.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gbblvlizf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcagcpqec.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwjftkvug.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gxgrqcazl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gwpfnzfbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxtfkfpoa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gywxqruhe.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gypsfursm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/genfrsoyg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gazldchib.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gplyysulk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gpsjacsgv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gelubprrl.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gluyqqrch.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/guucrpqdt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggmfcbnoc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grbnfmhit.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpgshjcrg.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gbvalovca.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gipyjlcec.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gtauehiij.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gudgjhgrh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gorugojtl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gxvqivnbj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gfkbwruaa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyakaopac.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gvgtzplcs.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gojoqkncg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gkctxkkfa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gtnaixzhi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gumjthygn.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gegwasbnl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gbgepqxel.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gutblxeyf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/grxzvymym.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gekbrodeo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvqtrkmfe.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gmuokipmm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqtoypxnk.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gujdftxpy.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gsxbkgpjb.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gudcixtzq.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsleftfup.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gpoirysvv.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gkwhkgoie.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gvehpiyia.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gsuxoweev.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqutiyzgs.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gjytjpbvk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gyldxeltq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gjlfgklbg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqyfawlb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gvfcttgtk.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gvktsbvjw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gztxoqzzg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/goavzpoza.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gdsplrhik.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gqdjeewnh.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gwlxvsgmv.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gwbdgltvw.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/guvmamkit.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gyfcoeqvm.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gywdftyhp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gjjzoakwa.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gieqsghuo.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gpxkflzuf.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/ghjkgtkjb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gcoraaanq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gimsmztdi.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gpgyzhzbp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/guzaoeibq.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gnsgmmegv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gwxbaxabr.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gtavyvbhw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/ghmrkwrbo.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/guomeppsc.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gaaitsadn.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnbcobxpb.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcgjzalla.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbfutxget.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gbyeaerxj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gplwkgnny.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/ghwwekhmb.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gspdqthqj.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gvssaregn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gayntkogd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gqtkzggwk.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjidmikik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gznvjlmlo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvfxriypj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gjnwzyvmt.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/glngqhdsc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gyuqwddwd.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gtldqpztx.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/ghglvvlhy.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gexuihwom.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gksazcbca.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grpbylcou.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gejtobvis.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gzfviwxws.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gkodnxuyd.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gayuqyrqb.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gsssebaba.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gmqjryvie.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gledhfleh.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gzxcmszlc.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gddwtxnzx.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gmjrfyede.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gqlyeuxzh.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gdawdlgqp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgpsabfc.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gopikoiaw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gftlfykwh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gkzftrbvq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gtyksiyrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/gzeiljsen.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gbbuxcgky.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gbipzolgp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gdpeailtw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gmacjxtbh.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gwdxcmfmu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gbsjgsokm.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/guyjtyzuy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gyudgtivb.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gexmiajsf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gnweexymv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gdscugypq.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjrkmdsoa.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gknbmefcl.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gidetrrlz.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gixqtbxhf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gpxtajmgj.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gdlykmztw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gksbxbhgp.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gjlqmgsel.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxltebhzq.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gonwmzbsy.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gmnrbzuyr.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gvielmndi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/glvynwjoa.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gnrzdsrmk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdometobp.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gstugckmt.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gyorfhhfg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gdoemsjee.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gjdqskhva.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/grkhrlerk.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/grhutwnkb.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gfinwjauu.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsjmlsxgt.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvejkbwqc.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glqysmhec.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfoqlufbj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gmxxixvqp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gwqgeoqvv.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gkuahtvsh.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/ggcuseeuo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gdzdcpkoi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gkgpdqrtr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gvpbnqhdk.sHtML


<!-- 参考信息 -->