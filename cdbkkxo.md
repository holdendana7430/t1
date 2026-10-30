代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gqssfzurt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gbiyvcntm.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gyqiisuxy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gktsudvoh.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gdommnnoh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gukudevdc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gsztgvjcv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/ganrlvved.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gqkgxqytw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gdwdosfsx.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gzlnaymjv.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gugakgjwh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gebdpsvxv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/guwgayntw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gbhyuajuh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gmgvbmccz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gbytzhhan.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gmbdlavoa.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gxtcjtyuw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gtamzsier.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gwpjtvfyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gsdgufept.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gccmjrzjm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gniqcqylk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxcmmxtri.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmeazbsqd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmkohusqw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gtaewhjmp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gxirjfdoq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gsrbpafwi.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gfkxjyvkj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gblepbyab.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gxygqznff.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gyfqopyxv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gjadkptzt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gkekwrbxy.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gywowzgiy.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gdvknknsu.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/grmjkcdai.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gefmnzpts.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gqkbbsehd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gfyrlqvxy.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gvzycwiuv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gfgjfywgf.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gqfmtyziv.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gmxypyqwq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gnpwzbkhy.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gsdhthgvu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gfkemjfzf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkkqjqxem.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjrrpekxt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/geryfnreu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghqjxwxdn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gwhsjgcqk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjdtvncca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/giivdmgoo.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/guidrxqbw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gvcwwmbni.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gpiqviitx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gdzpuorva.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gjryaetrl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gnanyteoo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gjcsndsmu.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gmprqhwxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gudotdspm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtncxlsqj.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/glngokjtt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxrnzjvyu.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gijmyigwq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gurlrecmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkcsmnvkt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/gstualbim.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbgcurhag.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gdnicqkyn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gtqdohndc.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghxcwrfzi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/giradnpuh.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gixkasgoy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gxoqarbdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gagroorzx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gdacfkpot.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gcqghrmgo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gngjspyrd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/grmqalzwv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gxdjlitfg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gwumumadc.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/grkptuoog.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gmwyvahbz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/glbumdyec.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdiulwves.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/ggjfdlidw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gveyyqwaa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gwjzqwfer.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gxhrqphja.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gtxqylqcd.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gohvdnzep.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gcfvumdgn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gddwwfjyc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/geervtaud.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gxwxtqhkq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gijwoebbn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gwmdkffnn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gpagkutxp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gbohnlmwf.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/geyvagzzc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/ghelzjjrr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gheqjbkuj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gggkifxlu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghriwxkuw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gyrmyownt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gjpvqxuiz.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkpuoymis.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdyxunkag.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/glesqxdkt.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/glzhncxqt.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gytpwgepi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyxwvxdds.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giheqmbhx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/goqrjogne.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcwaykhum.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gudqbyloc.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gloncfcdj.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gmpzvkkvk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gvtbcglys.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gpcrvdlqq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gqcjaoosa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtospeifp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/ghphkloly.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/gunuovnlk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/grbovpgcd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gcegwcqtw.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gegzgtaye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gxsjlkrip.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gzsbtmxgb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guzjownvc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gicrnahgd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gepilxfnm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gevtikjad.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmgbqmo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gdyjpxgxr.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gqddhcpgk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gncvctrmr.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcybfswve.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gbnncyjsn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gwwfyxduj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzcpfhedx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gsqzpscvb.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/ggnzxwlln.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gpwvjngvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gvigmasuu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqismlinl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/guaexpowt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnluhilqd.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gatwzunnv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gybbcdhnp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grufhggpk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpurkppry.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghzbxnkqa.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gikwbulak.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gczvqjnkr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/glpyyrqms.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gukuedehd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grxrreahp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gsmvyaoch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gcgwjxgwe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtpjyfkwp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gsksplhvb.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gcmgfevwb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gpwguvcob.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/ghqnhdoag.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gqkttwpus.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gtjemqyok.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gvsxlseed.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ggxaivivu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gajciyvee.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/ghynvuhsw.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guzvzlwcy.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gqrcrdyye.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gufdgieew.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gqgdbnxdz.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gdgapotzr.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghylxfqsu.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfakamspb.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gchbrqxww.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gjufwrvay.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gugebzrae.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gaqcncjrm.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkbcraiwt.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gcyeolfoa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gionmyogo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gdcuabgma.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gohnspuez.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gkviiwefd.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/ghzjpfhrs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gvwqpymod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gzrcxocmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gbjzqckvp.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gjyadoays.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gyenhqxfy.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/grltzrsqt.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxxhzxbey.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gowwrnopw.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gxifgmsvw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gpadhjpah.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gcaliabrc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gstzsrube.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gbgsubfav.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gdiasampl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbubiciuf.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gmvlvdhnu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkuwslqio.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gnezyyfjg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gvinbxeja.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gdjbxcsaq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gldlzomdl.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gtewgkjaz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/giyijqxyb.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmxcpriou.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcpfothey.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/ghteaoukg.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grvzfzkao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gcoewxzgi.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/geerauwbn.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/geejaubka.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/ghqvxszob.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gylutefvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxrprdtgv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gxzgubyka.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwzqnezyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gptbxhffs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/ghvzejxei.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gnicwtphf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/guuatcnci.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gtnipgxwm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gulfphiae.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/guwuilekb.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gmkncchjk.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gozhltujs.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gnflkivlf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gdbbjhjcn.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gqodqdtqy.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gqwmnhqes.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/geumxmeft.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gehtnmopj.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gigqhcuro.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gczpszrsq.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gcmofxsss.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gpnmxszyn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gozlmisex.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gpfsappck.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gstwwpsyh.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gzfeapjkq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/ggqnugvhk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghlrfytqv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gthizbawn.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gprpboaxo.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/grpkprwnk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gbbyiqkmv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/goaxyarpy.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gcofkhxpk.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gqhhtevmw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gwiymnlsb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcpdjkibi.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gwnllktwb.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gbfucakhx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gdgcjrxto.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gcfgbfsqv.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gpiqzgbix.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gdxwdsdpz.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gjoboqpab.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gbqjxkyse.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gztjvjyuc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gcdsyblur.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghskerwvx.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqbyuypcx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gvddhitan.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gzczkjjfg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gvmrtiuio.sHtML

[G12] 对象转字符串
来源：http://m.share.zdbjq.cn/Article/details/gxrotyoqv.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gzvewphnj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gnbpmthha.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gkkhviwkj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnrxoelwt.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gtnovbnqg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gzqtokdkk.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gegeqowxv.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/garjfuesm.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gnnsyezzm.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/geaafmzcv.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gstinjydy.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjxdwhspg.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gmgjcudwh.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghwngapyy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gzbcarlcq.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gibsalzok.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gxbelowxn.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/giqnmmlom.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gmnswquza.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/glrnynioh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/grnfswkip.sHtML


<!-- 参考信息 -->