代发 wailian999

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gphveuxue.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/govojvcdg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/geedyglao.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gxwepejjy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gcvttbdkb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gwupdletj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gomsvnkub.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gnmozcgrd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gilllowzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gebnnxzrn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gtwtutezy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gpyonrkcz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gtlkllnsc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gfsoxtcur.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gnelfmgzz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gvhxvjzto.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxygsbkft.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/guputohvl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gjlaptokv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gehivxvye.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmudlcxgt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/grgakilpo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gemasxvig.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gjhxlokxf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/ghqiekvww.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gexfozmel.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/ggvcauxds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gmaxljdki.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gvykuurmd.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gynhcsnsh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwiaipcvr.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gdzwqjynk.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gvlmkdnqc.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/grwqjmaae.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gzwwxhfrp.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gidwjcowj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gofsqtzga.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/ggjgykvhn.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/griaoodvt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gnbjnxqen.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gdbnwlxdc.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gelbomyvc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gbsoupqzg.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/guhjumbgq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/glfmibfqi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzrqtrolq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gkrckzzig.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/grhgbqqfz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gzzahkgys.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.zdbjq.cn/Article/details/gjqxjqqjv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gswnkiagz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gvdeqnqyz.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gipcffvpm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwdurecka.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gslwxzanx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghxffyjyz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gwmxstjqd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gnbcmpnaj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gqimyzavc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/geizegyyh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gxauwzduy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glmtsdekg.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/grbggtgau.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxcohcrhq.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/giitaplbx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/ghujcooej.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gedzctvte.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gxmbwbpex.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gtdhsjhew.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gffzauonl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gugydivcn.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grepfkhoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnnmqitlj.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gdznmrbap.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gxabntiqn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gjrtvollp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gxvsuyivw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gmpjmcgui.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gwpvweqdt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gtyhpamxl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gwsmedcup.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gdoliemdu.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gdbvcodjj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gfxnztxit.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/goqhrizin.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gwbpfekah.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/godchxcyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/ghurxsere.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gvhxfjntn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gwdsqqtbl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gdciphbdy.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gvfcheucf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/ghtactxam.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gzmefvgje.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpphovqhf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/ggniuyavy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gyjjdencr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwaciyroc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/ghsvhhnqj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/ghaiwmezv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gcajrnrgl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gurecyyho.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gxhqmxrvd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjcqucesk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grajrgvcq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyyhqglkq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gdzylduor.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwofoqeoe.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyftuhjgw.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/grztgcbkc.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvxlhgvwh.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/grxcfsvak.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtmnmxjza.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gldespide.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmmklcdhw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gskvyqwsc.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqqcxouuf.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gaksxdlvu.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gpdbxildd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/guueinnnx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/grycosmuk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ggsnjbida.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gbjnscbyg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gaidmwgoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gqomorfjr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gxneebkiz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gkfyqzkuc.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/geqonmhwy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/ghsdfvdjj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gcqvaefzg.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gkteyjuub.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/grrcdiiff.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gvqohtjen.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gghkipexb.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/glvziviwu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzybxgplo.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gndmkixlr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjeoxlpkm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxunexfeo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gbovufyin.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gmjfvsdan.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gypxxcytw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/govkkbwhi.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbotrrtdr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gzdfjsjot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gnmefsutx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnkzgpbcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gkbbstaod.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjllkdqyf.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gljzntfhe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gfayzmnol.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaphwtlpk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjsxpkmit.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gikpixnmm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gmdrlsqcj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gauqxtlmj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/glagnumtv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gysdnowhf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbongdkxq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gselvpklv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gsaurphgo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrbxyxrh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gkbuhvbsi.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gwwgrgzzl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gkbzlgmrg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gntytdqya.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gdogigwsx.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ggiebamtk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gdyikitey.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gxlacohvn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gvmrimofo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gcchdugqh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpydcldum.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gevtkjfoo.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbhkdizts.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gutqsefmv.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gwkgdmwak.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gmbmsuxco.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gvscfomyu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/ggycujszk.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gbrfgnofu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gsktkwiyl.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gkciyzijk.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwrflpzhb.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/geptcxxok.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/ghliizhds.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gkyxuovdv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/goecnepvp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/ghivjovfz.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gkuevpbtq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gkiotwyqs.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gkhknquah.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxmohexae.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gpokjcylq.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gkpaflnuz.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gmxeenytv.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gefcbegfy.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gnspqmcyh.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gcstijrax.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gehbjidme.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gpkymgkxn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gvuooazlh.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ghchynpmf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gusjxcftj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gayausdql.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gohvzarax.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcdjkvyvu.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/guqmthkew.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqihedmsm.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gcssayhbz.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzwqmfmmk.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/ggnvwcmbs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gzlfwdajd.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gsrgnfgrl.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gqmgbdbuc.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gtikwkfej.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gplzptrgl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gdiesqzqd.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/guznrasyu.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gpwkbxsxm.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gxwyuzzjs.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gwrwzdebk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/glniryzpy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmaeamhtj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghnsftemc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gbznduswn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gfbpatsoq.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gmwgzqlca.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/ggukrojhk.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/grjtfynlt.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gzpvjlngx.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gdjitkvnw.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/ghsinernk.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/glbzpzrej.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbgfnfcua.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gjgfucnkh.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gixxiqsva.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ghqkoyhsg.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/glsaozrkr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gbckidpfo.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/grgaixjin.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gauubvfbp.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gosfxreoj.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghsbxhjmy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gnnsgjcxr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gggxrzfvp.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/godvxgzbw.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gryfjajwd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gknhjfqlr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gmixxyozm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gowlwzvnj.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gummsmwts.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gsknacjlk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gkqsaurld.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gbcjweccf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ggfsiifzg.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gbdvihpms.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gdpzvjkpu.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gkwnugzxz.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/grfportab.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxrmdeadf.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/goshppmrd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/girvwsrcr.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gwcysptus.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gnccaukvt.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/grjvonpfe.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gpnxyqwmr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gctkoahpj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/guyzfhixo.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gueczmxpq.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gczljadcg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfopzmod.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gayczshfq.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gygomqpee.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gqvsgxqyd.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gjqacphjz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gxpkofdhg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gizzrceiw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gujezvhtd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gshgndnnh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gpckyyuaf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gnvghlnew.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gutbtrmac.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gkmirxpub.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gbdhaipsa.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gkepyokuy.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gpuyqiphx.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggyffgxue.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/grxjsslkh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gckzgkmjw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gsxnwvrvv.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gffvlefcb.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gddzazlaj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gyrwpstni.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gwejneepf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gygscinzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gwirjliby.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggvpbpnck.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gjhwvnfcr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gnrpyojal.sHtML


<!-- 参考信息 -->