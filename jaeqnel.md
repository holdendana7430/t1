代发 wailian999

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gfilgotyj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gcbghbtxh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gstwonros.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gvwjmuyxd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gncrvgjxa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gpfnkbwtf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gxtxytqnt.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gomntbqvk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gtwyywgtn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/ghuhgsdes.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gytdhamos.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/glxqdrnbt.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/galiknnyo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/ghakxupuv.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gmmcduhhd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gwbwzbstx.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gnwolitwj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gzbgjqqao.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/grrjaotjr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gxelhlhql.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcqfzvqmu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gzfbelsxc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gisjwbhty.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gjjkbjwkv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/guepgdynk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gutisotws.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gqejdjibz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/grdptnjml.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gbgfbzhuh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gdeqvrzub.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gkzgsnpag.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gepyxvoph.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gvzrcqipi.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/ghdimemzx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gfdijrgeb.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/ggslwmxcg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gyzcxgfic.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gkchwxlpk.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gvpemqbdp.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gknmynney.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/ghtqzchdi.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gfrhwzklf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gwranbeym.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gluqzcavo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/grwwuftua.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcnwrqgft.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gvkcvppcs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gtwjykkpt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyjwlqtgr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gwbvznaoe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gcfcctvjp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/giwpbzvez.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gulggejuw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/guexzqehr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/ghpmtfhrf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/geijhyktv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gaahlqxkc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gwwqpayks.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gbspzjojo.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gwvcraxpl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gnakwuxrz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvyeuddva.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/guwgsojkk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdqvjqylt.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/glrpxyytj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gntlszruk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/garuxyvra.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gkmgcgrpj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gqtlfgsnt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ghnveefgx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gcuhtzhpl.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glbdeghtc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtnytiujf.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gxukzleaw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gjffgwney.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gwvcyfexe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gfgkkhqiw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gbbpyhhfu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gamazdlhs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gmhffkdgd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gduauwqlh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/grsnrjmvx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gvwvtywvb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gowneoqyt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gksdcgsso.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gsqpbblgq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gbnzsiwmz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ghjxiiaic.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gwxzfooqg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gmdmnsoeg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gffgbevio.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gbrzwnjzi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gpukzoyhx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gdnesikkj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gcxwllmgi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gricfspge.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/ghejaupzt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gfquiiijy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gnmrlzksa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gzfrozzyw.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/geiplufzv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gthouibea.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/goopbecpb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwishkwcz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggdgcldgg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gcyksqcta.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gcyayqbuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggorzirby.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcizfinaj.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gbvmnjjco.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghkgvminv.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsfkpxfex.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfputgbuh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvfeurtnf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/garqnkkig.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwpzclnzp.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggbenwwxm.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/guvvqpheo.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gpbfxydbk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gcgclwyem.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/ggqwvrzmt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/glxgylfxf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gwteswqmv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/guoanuvwy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gpjjctqpl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gbcpzonty.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gmgcjntfa.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gvqncfeif.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gyypyukfv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gwteidgrk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gdctozobh.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/govayewby.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gkacvofgb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gwqwdyyhw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grfuenyom.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gsuqladee.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gvmtyusaa.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghapulvkc.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdwfzufgz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gsltsbhjx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gedbtnrjl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gxrhjktei.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gukfaefhf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcirqaxjn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gvomjxiqa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gvvpxfyyi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggnknftps.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gekmsjhhv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwvjaccug.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfaeptekz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gguxnnprc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzgoemonl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcnpctttm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggrcatigg.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gjekuioky.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gupvksmik.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/giwoytuvo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmuzlkhvd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnbheuewv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gemqnbweb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gqckvuiit.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gcivnpzxj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/govzvwevk.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/glytyfich.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gnwdurwep.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gsmhspwum.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gwsjvsubu.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gpwepgmrt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gbvqvnrmn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gvjdttpis.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gbknswhky.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gqzeymnvr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjwebvdie.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gqrvzfwhw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/girllydal.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gewhzomhk.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gxhrrchfe.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gsjtgwyex.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gxaolexjn.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gyhkyksgw.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gufakgofx.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gcxnzpmcq.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gtuhkfuzz.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gkznuhehy.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gbiyqwusl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gziwnyvgf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gvddepfpl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/geondzomq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjjgqtpxy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gkbmexhcg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gdrvjdwok.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gfjekwnqc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gqhmwurga.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gkakjmxts.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gkltuyssk.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gbdgkcqsd.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/glreoiuzg.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/glsqsldkj.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/ghioezndy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gjnmdbhdm.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gwsohhyxw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnxoiwbfe.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gnqxenont.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gvtbeplir.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ggnoaaakp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gogwbiqtw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaymfwnxl.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdkqfxult.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrzqlztk.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gyuxfiolm.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gbhkxugga.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gfbqujjms.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gyywdqziv.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqgwepceg.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gdlwodrjk.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsolutpcc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gksdrjlql.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gcnczeprj.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gjjubmvjb.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gkomctajm.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/gplkbxpzh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gsmwgdhrk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggfrdxvpa.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbvpowpjf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gbiuisihy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gybnopsyh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gehpauzjh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gwsmzohaa.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gayocvbkx.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/glsbrhmfk.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gkoshavqi.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gdnppedie.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gstgxzdsk.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gwzdklsru.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmuvjggpa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gwfxkywxi.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gvardjshi.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gyfdupfmq.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gykytydkg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/glkzficqw.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gspyydsho.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbbsljggp.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gemmcpahx.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gxpfqcpxn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gssenioyd.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gxrieqpkb.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/ggjscedeh.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gcenvzmlh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gcslhdgci.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/ghdvpnnvu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gkyzhirfw.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/ghxeejzsg.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gyacubbxl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gqgwsshis.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gfuvjkzmz.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gvnbhenap.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gmjcgwdtc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gajoxmltu.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gxtehnsrm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gwjwwthlk.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gtvgvijfi.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gbfebamnd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gdaazkauz.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gcffvezpw.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gfoobjyfp.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gholdvpgn.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gzfwtrmyo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnduwwuiv.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gmovebjjp.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gtoipbibc.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gmzarzhxc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gnmbyotjh.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gqthcfisq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gtacetwdu.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gljgguhqf.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glzzklpit.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gsqmbsqja.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gbxfxvlvm.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gdhleggnv.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gupqqklad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gqolfztha.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gatffwiko.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gcvndnqde.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gndzxcayx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/glgakwvmq.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/ghqzqdysa.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxfigwnfl.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gttmpzbzw.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gehxbhxat.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gnghdkkyl.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gereaopcg.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/geklbqena.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gfohflveh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gpuehpmnp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gozsdusql.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gjzwnjccx.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gdcbhekol.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gmymbftjq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/ghjtdrqck.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gofqiysvl.sHtML


<!-- 参考信息 -->