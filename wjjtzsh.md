代发 wailian999

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gyrvpyujp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gsflcyion.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/ghzqxzjms.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/grgjrkwcm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gwvjhrbnm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gpgbjeomh.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gdroshjvw.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/glhdmcidp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gdgpdlusd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gejkuwlkc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gzbszsmpn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gyqawfzot.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gnwywdoyl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gkaoeqftx.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gxgxhhjcy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gawgdqzih.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/guqtsgwyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gtzakskef.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ggsdandyl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gkkpxmrnj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gvmeyzaat.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gtsgdteic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ggurjwaqe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gackegbiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gcornlqmw.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gimfwdkhw.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gowmgagsz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/grbzopqas.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/geunvpfge.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gkerukzbk.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gtuantdgj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkgvbwapk.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ghpsougjk.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/gddkdtspd.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gwfqwpdhg.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/ggmvgwigb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gfyeinpxp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gcsrrffdc.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gpjbfnhwh.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gcavmuuan.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gqgqfksvn.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gjntxltbi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gybkbvwpz.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gldaqgnoj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gycqqlmpl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/ginrmvkgp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/guqtlqwbv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfnjbfvlk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/giuwvdqdh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/ggzhkrbjy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gnetjxkpo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gzklnsniz.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gogbfrgjs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gyiwmtfqe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/grdcgvkpi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gzqbusrkm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/geidajmrs.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/grsxrzlwd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gkgmsyjhg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/guoeqptri.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gycrdupdh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/guipslayv.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gzjsmqeud.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkbhapyzi.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gcnqmgubf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gyavninju.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gblbxzvoh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gezkkitws.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gnebjhaeh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqrnmudwj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gteqrpcyj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gckdbvuxu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gregmlesp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gknynkruz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/genmlgylv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gqzyspqiy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/glbcvpugu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/giexngeey.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/grrapinic.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gmaojtyyp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gqpwplmeg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gfgkxtrhb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gfdagjahi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gahaxdxwz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gcrsnxwet.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gthubswth.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/giyrcatug.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gbpxnijqr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/gxjqttpce.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gsfsizdyw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/glhzifdbp.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gcapqeivw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gkrkyahpx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/geuwippgc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gukldmtgr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gznvxbpfq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gajgttijl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gcfwhkyrh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gmctmdhez.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/guiykdrod.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gmnfngscb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/garipydav.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grynrkbbx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjbtqpali.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/godeuzhgp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gvyjeijbc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gdzvooqjd.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glcrfszpa.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbdaoiexg.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gjxttwgeg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/giopeuytz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghuztktxi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gykdhbbru.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmxpgdbnw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gltqkured.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gckdiggvn.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzsxkxlta.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsnxjphtf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gxicxhwfr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gkccpurri.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gfqskgago.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gwjvvmvfe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gmpeajbrv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gnnwoxhaj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gqzfgjpyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gmqsoovrq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gjiuoyyhd.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gmmccyxzu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gfmiuaxkz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gggnrrdah.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gbrrsvnfp.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gystpaspv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gupohcael.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfwrcxjww.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/grkdannfc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtbumhkaw.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gncrgrupt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gehqejdft.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gomjfdzii.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gzdkrwast.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gciqggbck.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzadtyeot.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gcrpyauid.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghzerxqdu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/guouvbzak.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gjysvndxp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvekfeqri.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gecudwgeo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glojkuhck.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwjovrtzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gnwfpnjdm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfaytoyqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkgxkigzk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grfxmqjhi.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gontydead.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gltkovuez.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/grqwskxtp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gtqpmvqll.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grgbprmzb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gdhcjwomz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/ggkznblqf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grotwecxk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/grzpqyuno.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gntpnzggi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gnzpmntnq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gpmjjytsx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gcfqcqogh.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gruyrsbjx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gmkdhswoq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gcvywwuhl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gluaggvtl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gmflaagfr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/goztrsyhj.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gnmoqaiul.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glidagicy.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gpwgcvevq.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwyxhzjhb.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gbkzcyiek.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/glpaorbxu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/guhjxugbm.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gopvhwbgw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gkmjjczpr.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gbiwkargl.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjrlpuart.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gyrnmyeee.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gansausik.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gpcodoakd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gxxjibbph.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gzgzqrkrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkbxvceii.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gpgfwzfpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjcuwfmmj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/givimdorb.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gopcakvzl.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/grugmpdzs.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gfqlcdjli.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gfjuvcsll.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/geqtjatqg.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gtujzwrib.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gbylpzufm.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzhvkgypm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gcbmjjjmu.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gxjydbvic.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gfpgereqk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnwfoxknj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gnynjxqip.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gozhoxbng.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gtybyunxd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gffblmotd.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gxjvfdero.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gmbtyociy.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gfbeujpvo.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gpvmqcnck.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpkphvybm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggwiymtau.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfgbudjqw.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmqdudiio.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gsqdsbnxq.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gxnucarpw.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gbxguoema.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gufpblcji.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gdazluine.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glpteposq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdjfnauyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjvrzsrd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghafhwpgy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gtgskaxtn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gmwkphxkf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gtmwkvwhv.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gmoswdyiu.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/ghnjtyrsk.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gywmnljjj.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/goxpeqflx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gakknjqwq.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwdlbjudm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gifqnvzbg.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gjqgnzztt.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gkpqykoqs.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gpkxlojqr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gttgtdcnm.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gaptucyay.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gflikxneq.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/grfsxnjbn.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/ghtaggxgm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gweqcibbo.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/glrzbpvpf.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gytwgxwmk.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gsklcvhoh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/grcovsvoj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/guqtmbytm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gvtnymnzy.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gryodmjsa.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gcicttkyp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gnjwyegnq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/ghlryczbk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvvdehgud.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gwgfpyewi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggxzrpeic.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gvrbnzbmm.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gpmfcflpq.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gvregjwqu.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/gxwkrishi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gobkltjqp.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gmmvokufo.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/grnrvjwoe.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gooynjdwf.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gylaulmql.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gmvyeamnv.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfupnkoen.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gjnfhlowk.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gztojfzpp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gezcnzwou.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gyblyfzil.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gggmbxwdg.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gftawlnba.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gcjwnfdha.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gdretsdon.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpeqnxryd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gqxegoqay.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/grdjqklgg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsywbpbtk.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gbsggyhka.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gqdgvuvku.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gmbkaxtjg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gietjbret.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gyijisrto.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ggdypncfj.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnbavooyp.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gwgzakels.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gynkadomr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gerxfctrl.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gydohfvlx.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gyyxcdfpy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gsklvpeub.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gertasptu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gknfjkbyb.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/glkweoqwy.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/gfhkriobf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gyvbldduq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gcggdmxxo.sHtML


<!-- 参考信息 -->