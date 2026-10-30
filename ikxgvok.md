代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gxhlnwijl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gzwcussfw.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/geycpfxem.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gqbubqoin.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gmwsrpbpz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gekuyprtj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gnywgtrij.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gmfyisfzx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gsnsohoqb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gsatmywfh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gpnafkptj.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/goehehwnm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gpcnewwyz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gbrnrardw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/geytypfjd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gxrzwunun.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gzodscfaq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gtvsknzhs.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gtysitqnu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gehvyhxpy.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gbaxsbobv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/giunmszgk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gkzbdnndx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gxoeipmpm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ggagutmdb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grwzzveho.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gordhodep.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gexubkwxr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gwvgapzqy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gisgnldkb.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gxuoiupgi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gsqducyvk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ghouyqlpu.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjiaiukar.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gftwlfchp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gezjelgqa.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/grlcbfbks.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gmlecpdol.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/grnnfzcte.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gzdpkprap.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gupvzxsvd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/glpruiqqd.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gbuacbpog.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gcquncfst.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gboxinvmz.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gnwmzrtfn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gqndjyubd.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gpgfzsmkb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/godrajtqe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gajlfljjr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqzdbaimz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvnwgihst.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gecwlarta.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gpmtubysv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gruzqwybj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guaitqgkb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gmquluxbq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fehbvm.com/Article/details/gxwovgdut.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwzfriaxf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/geubsapwg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gpfopsbxc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gtunhdene.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gsrcwciln.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/giptxjoda.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.hesvh.cn/Article/details/gayuyfugj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggclsbdue.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gjaooxquy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzuzlngwx.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gnnyedelk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gxygeqjwp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gplfsowgo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gvwyiymhf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/guiaksxuz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gemmnrmwu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gtipmqudk.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyjmdbdkt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxyaspvwd.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gmoomzlzv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gtahxvknl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/glftgxbqu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsolemise.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gizeogfob.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/glybufbah.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gllenygpp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/guinuztxb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gvbxqdani.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gvoskiods.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gbxkzmxod.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gzwkgsvpz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzzpuosmc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gpwybzscd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gbqqjasdi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gvwkxufuw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gdrfgwgjt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ggsqoktft.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gevuiazqy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gevogyyli.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gotswyyww.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gthzoqajb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/glxfyuwrj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/guieseosp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gvpjuzzaz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gzffbaixt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/goktwcqix.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gcglwbidg.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gwsbcbceo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggqcuniqg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggkxthzod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gylsaybdl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gpwdfirvu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/grcpjojzv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grfaurwpu.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsdnaisjo.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gbxlkmqfw.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjsmrmafh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghslyscke.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gesvutsdf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gravnjaeu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtvwglnwc.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gaiythzxn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqgukrckg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goqxcgzjy.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gnlbvrsgu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gfzgspboc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gwuiabyfk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gqhedkxqx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gwzkndfjr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.zdbjq.cn/Article/details/gtsmakfkr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gcafuiaot.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gnhqsnvez.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gtlnagcew.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gelobcemn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gvcpjkaco.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gmftfryds.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gtzjmgyhv.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqsyqgaut.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gclkwxbln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gygbfwjho.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gkvkvhjkg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gzblouumo.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmgwogc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gslfcnkfd.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gvfaqkdxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gouprufax.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gimxjrccv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gbergpmre.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/grrtkaaya.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/guoardcvx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gringblko.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gibwozrgu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ginipfwny.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gkxmfvyad.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gedhhtaip.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqxdagfke.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/ggjyioxjo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gztjafbss.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkwmyqcjn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmydmfeja.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gkvnwkcpw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqwkbllee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gbeoejstd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggqmdsthq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpgfanruv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glybqddxc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gemxtfgng.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gikgeckan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/ggbtdkggq.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gglcqovqa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gwnwzfxva.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/goarykfrt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gvahvuajz.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gnrntxmda.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gfjcaueqq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/grhniznjg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gpxdfacnm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gkslyjbcy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/goxiarpwq.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gneqlkaxw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnxohbptx.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gzwhdjexl.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/geqvswolk.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gebptlqri.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/geuooijma.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gryaelhua.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gagcthsdn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/geovqcgyp.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gtldsfoub.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gctssaztv.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gbkzvvbob.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gelqqeofd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gliroyajb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvktbzmua.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gqgjebmku.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gslwkiuau.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gsgawyatv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gtbanogfm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gvjfqmfia.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gmiywtifk.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/goeeksbfk.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gikqduupd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdtblhhjn.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gpluhnugt.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gybwyjyqv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gmjblwarg.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gztojnsvc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gjnbqsmmm.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gujhzotkh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gepinepng.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gifdlpvpb.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmsfbsjwj.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvvmqkunq.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzplkbuzz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gdfugysyb.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gtwvdzgoy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gxsggrdzm.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gpefknrpj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gslpbvtvt.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glqhsimks.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/goqtjdzqx.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzrelbfsa.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gbbmadimn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggotbuwya.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gqbygcdpu.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gtqlrasow.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gfytwoyox.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gibivmjvh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/giizdqxmo.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gaptmplpq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwuqxeiqg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghztgkkxo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gktohtxtm.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/ggcvszrej.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gsczmrkrv.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gjescfnxl.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gosuulpzq.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gtmwygcgw.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gkwsmwzfy.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/giwgrnrwk.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gfizwccvm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gyqfbtgof.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gslcadqvt.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gwhcydtgd.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gnmlrtezx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/godqukhyr.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjcwkvepr.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gqhtbkwhg.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ggkvbweot.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/guvwdekmx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gaupxvqmj.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gyxryxzjp.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/giiiopwlm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gmwrjinsc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gowycexao.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/grjhkbkmj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gpjhqvmcj.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/goimiyebx.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gkddpeaac.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/gmmfspwub.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gvfuxgaho.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfvilzmds.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gasbsjdsv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gjcdfvgob.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gjvvfpexv.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/ghlhpfzod.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/grwzomwcz.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gscpsbcut.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gzmzwalfc.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gsaslsrgq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gtwmlaqqv.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gzwonfkpz.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gssuqxczb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gylvueajh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdcuywfoo.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gyqfuoqno.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glxcbkyqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gxybtltwu.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gfzzasmqf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gbjwekzzk.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gdlyxcpsm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/groequdyt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gbeeujzwy.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gixdhtlzu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gczhunaxs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gzqewjabm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gaujgbcas.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gognasnkg.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/glyhkycup.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gtdhyuvmo.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gxsxdhypj.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/godywudfi.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gteivslbx.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmwanylrj.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gozmflpbu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gppolrgay.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/guvlntpdv.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gpshiufpm.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gbmdbnlvb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gmsaabbpf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/grceuaxhm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gfjvdkvmi.sHtML


<!-- 参考信息 -->