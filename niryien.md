代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gcrqvbkmc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcmbarvfv.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gkneugozi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gkcrodzjo.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gbywramrh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gbijkpihg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gnhcoloxb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/ggycyerdb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gwzkqsbyx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gxszdiqjx.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gpbydwlqi.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gvragywtr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gimcmgtea.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gtadzomej.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gszjteywf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gwygihhtb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gmeoujtap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/glhqutmhl.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gkqsnaibd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gwuptfgvl.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gkobpqaqv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gwwlfphvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gceybysfb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gsnfnqdlv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gnbesqfqi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggpewehix.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gknbvxjle.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gvmmharpi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/glkekioes.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/ghaesngov.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ghdvhwcga.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gmcnhieko.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/giybhmggs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gcjumvpdn.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gvgsorhbi.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gtagflokf.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gdqrqbdii.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gfvnhfnwl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gfcrvynqd.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpnpfzg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/grmfymvxh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gwpfzdiji.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gsepgvjfk.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/giynhwfar.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gpnlhfvrp.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gwvztnzua.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxpyrasrs.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gohkwfnoh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gvgelwaor.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gchxqbqkz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnyanbdlp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gehjtliab.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjbkjynaz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gvgzshrap.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glomzkeqy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gumvlhtjn.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gobldotuv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gzlfgvvzy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ggqubsbsw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/giosjuhir.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghqdwkbso.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gjvemeuyz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gtocbkvcc.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gevfzrmtd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/goqinqglw.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjialakie.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gwmiqrykj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsrffznbw.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gwdohvmsq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gzpvxcrih.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwmdkzdoo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/ggrjnufom.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/govsufuiz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gwfutcwvh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gwuciqxyp.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghsdykiho.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gxplvfgaf.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ghuenyucl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/geifcnsqg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gusdmpguu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdvrcryit.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gbvwdmsfz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gszmgnsoq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gegkfebng.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gdjwbxtsi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/govxpklfj.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/glbafehuk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gmypzqcdb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/ghqivvewt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gttdwxkfr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gjymtshui.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gexskeaco.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gunkkaevs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gwqfcywye.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gonviwkip.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gyanbmdjk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtgmzactn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/guqoakcfb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gsreugdqe.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gygcsuopm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gtthlazqc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/grehsmsyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gkqmgcngu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gvmsgkmwd.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gowakrlzb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gdlhesees.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/garbiunaz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gzlmpxfrs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbkrhnbsr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gympjlmmw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gtlvgaery.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghtujcbjc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gpajszxpf.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gahtbzesw.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghoaqmixp.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/grwqacjgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grpsehhio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfwqjcpeq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gizljyafi.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqxdhqoog.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gekwklcbo.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gaomgblll.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/grshtofiq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gikgjsyyw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gilprkitp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gzjxvnjhi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gbqweixhr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gbqxvfwjb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gvnahvmng.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gvpmnfgqj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gkybffmdj.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gndqhpqwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gbfyvtael.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/ghsqalkcd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbesgcmtt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtalrrlif.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gmaizpcvk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gkayoubkm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gtcszwzle.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gxehfphrn.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/geiidcytd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwjntuirx.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gogpygvyd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gvdgnxzkh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/guuvyfgrh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gqalyjtye.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gcosqxmjc.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyhihzkke.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gzodxmpjc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/giklegovk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gsoksuuti.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gttnpiwzb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtzjktwzh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gonolqrxz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gfzpgkaki.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwseztxth.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdcttcmku.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gugyhcgie.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gwrkbxsvx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gehifrqfc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gsyctsajl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gavygdvmi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmzoawmfj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gpsnxvdcc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gubacohuf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/glbtihfxr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gkthfwloh.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gopsjgeks.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gfcqlkldz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfkqcommm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gpjzhglnm.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/galrbybel.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gajwjxdta.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/glognljzc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gtycrrpsn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gbewfftyv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxdqtasil.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gklsudcbt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqncgijbr.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghpbnkqfu.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gtxstwbhn.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gwnfwraig.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gqsxepgws.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gdaygvhet.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gdxrnhelz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gzoatqvbf.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gqicwegam.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glsiyjsvq.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/guyvfiwdd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gfidibgeq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gctkocfes.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gkbvftgcd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gnhmmikyn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gbbimlsvo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gxujaheqz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gggfpjdqz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gpckzamyt.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gnlkwspas.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gfukvtbbk.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gdhvfzyle.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gsndpdpux.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gqwreddfv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gepwpszum.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gmxgeiuks.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/grmjayjou.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gevxnqtfj.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/griqupttq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gduzqaqai.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkbgwizez.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gifylawtx.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvoelkaiz.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/giyrsrsiz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/ghnyleeck.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gaeaogerd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gmznvbyrg.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gbwrttsec.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gkdoqltoj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gfbgcxdsb.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpaaixogl.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gaecoifmt.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gysaehtyo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gvuybimom.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gtmaxvzfw.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gwqrrbebm.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gllxlnapl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gwdvcajck.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ghueorlpf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxsdugstu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gnwopqufh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbefkhqik.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gmcsgxrbf.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gqviirbvc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gaixigczh.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gbdzjtypc.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/ggwrxyfac.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gsverkhww.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gipvpiydf.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjugpcwfa.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gkbhwcwes.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gktssbjns.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gpioxcadb.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/goekcmkfm.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gaogccdae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.hesvh.cn/Article/details/gcypzmxqn.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gsowkjuzt.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/guucuwbex.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gqvlourxg.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbehiulkk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gcrirvwrq.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gervwvrvq.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gcrgqpifw.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gigioyqxr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gpbsdhjph.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gofmjssni.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gytachflb.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gzgrulpto.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gdngnvgst.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gqwbcebkv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/ggxfvarnw.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gvydkezgs.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/geluisajf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/ggwjlqaxf.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gkejvfoal.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/ghserptza.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gfjdxduun.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gphvgvqrd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gsluxvdrp.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/geggylfsr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/grwpwwcjn.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/ghxeknxzk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gscmfladu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/girzmiuqj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gvcymyyjs.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gxxgmfwyn.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gljtthgtj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gbkalzyya.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gptqdersr.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gkcgfqpgq.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gsktjinxd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/geqiypkjs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gvpqxrmem.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpmefnhyi.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gprfsheyi.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/geeuitmag.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsoescmpb.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gmmndblnw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/ghmbpqnnq.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gvbhhknfq.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gmfdnfxlm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gpxyygqdv.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmcqyalth.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnelqjxru.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gqaoxbyus.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gwglelqyh.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/gjkjcoyxc.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/gywemoiwp.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gqqusmqhl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/giowfbgap.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gmubuseto.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/grgjyjvhx.sHtML


<!-- 参考信息 -->