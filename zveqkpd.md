代发 wailian999

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcaasfutk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gcuawszls.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gwhnchelb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gjwfqaboo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gyffurnhk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/goglzbheu.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gpadxhnub.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gthsywypw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/giohdlzyh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gzcwcsdbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gkcxqzfsd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/grfvauyuq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/ggtcvtqpz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gjlhdtomc.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gxdbwzldr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gvsvrzzxg.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gqagsedmd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/goymimqch.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gbpqzuixo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxferheum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gqdvnrkcp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gftoceobf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gxltsvwwj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gkyuqsqiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gshounaop.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gjustkdjd.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gjixklpnq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gonisosph.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/grsojoqhr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gaggkqlpb.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/glgzeuikl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gmapunglv.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gcgwgnnki.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gjpgctbug.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gssqiygbj.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gaazvacxe.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gdtonrovi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gqhaljfzc.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gbypzfcej.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gyuwybbfp.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gqehdhnov.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gvtywrorx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gwoxrovim.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gluijfxjm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/giodaowis.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gdxksbtsh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggqltdlcq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbthzujry.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gguwwfvfy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gpmbaxthp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glwghxupa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gxfaybhpo.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gdtjbsxdr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gnxwyxxgw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ghoepjkpp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gvtzqoffd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gfypbmsth.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gbrlrlgre.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/guqgctaio.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gagjphuhd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/geoizmedg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ginbwdxwb.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/guofnqxfc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwsgtbklt.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/ggnueqlzy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/ghaylgocc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ggvpsslav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gsxduebej.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ghkfysjis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gbwetbyfc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gvutpjmhh.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcqbcnpnl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghovqidvc.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gmktsltoz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gihwyjhyv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gsczitpfg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/guyhxoguk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gvxttnaok.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/girdfbbss.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gftzwjebk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gbhphkcnj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gtbxdgsoz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gsvoaexng.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gkopkmsah.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gtpqkumzt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gnmlmsdxo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gkhclbjsw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/ggoyugoxr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gshydwxmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ggcnfzztj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gbeyuscrx.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gglhojnsg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gepncvklv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gycrxuoic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gcjyspzdc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gdyuzuqqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gwnwopwlo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gtapmlktz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gclogutvx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gyzytcibl.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gfxopcchl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gimuiigju.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwkgthhbc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gybddqncq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gddycxvzb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gncrryvqj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gimtpmrfk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdqoynnkn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtyduqbgx.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gkkheipmr.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gloankvhx.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gukrkunuh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtfkwghdj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/girzvghtm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glofljgkp.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmoblokab.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gznsackhd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gttgaerii.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gywhzgncm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gmuenahnr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gxdnjuvqz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gjgyfrnha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gdnfxepee.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gfcncscve.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gpxsvpssh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gvrsgcsta.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gashawzpn.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gjkaftiwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/ggcwkrzad.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/ghzxkacmc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gobjgifhx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gocwjkzac.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gyhetgvwf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gunywyxss.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/govqabxrz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxsviagic.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/giaurlsxo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gydbgyulc.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcoqwisgi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/guodubccc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gblzkbegb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtmmominu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gvhgaaqei.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxbswwpog.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gulyxhioj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gnbttcnzr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnqjdldui.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gywuhnuhf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gijhlkxzh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfqdlppnl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gmjswzcku.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gphvxhmnq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmhfdvkbq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsuhggcgq.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gyukgpgyj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvegwlxpw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gdwadntze.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gfagzspuk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/grfuyzxnx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gvwnbgetw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gfjimmxlo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvvlzguvr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gghoipbpk.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gdnxskiwa.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gcrmhrshf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gsalzgppf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gitzvpsvu.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gehzyprrj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gcknjubij.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gisijwgft.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gquwrtpgo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gszlypcpe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gufcupsam.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gptooijmf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcpkxizry.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gushrbumy.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gppqikvqd.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gipuwbkjx.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gbbzeoqyi.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gomgunatj.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gnichvshg.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gxifwhnra.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gtmljwasf.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gaecuqjiq.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfwkrkqsn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gmyzbtkwa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gatwlyibo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gsswtxzrp.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gpootnknw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gddesvbyz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gcesuljpk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/glnvstqqf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/giycsnvtb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gjkknequk.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gqxcgbspy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gawuypqbu.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/glczpbstb.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gbzgbeeyk.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxuobxvgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/ghoxzqhad.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtxbrptkk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gdpcxydcb.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gzefclrwt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gumjbouou.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gigzaepqk.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbtxdcaqx.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gpjmvcryq.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gybjxeutd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gvueqfqvw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/ghknwxxtp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gsovyzpmq.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gqafdodqx.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gqxtduxed.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyillgppo.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/godvoofbf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gelbajqcy.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gorcgdxls.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gjhmyzjjk.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gukvgdzkk.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gnonjjfga.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gidozcsrx.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gzxwtyymy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gsedceqcc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqrglkdkh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/glwwqtxpr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gylktkzcj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/guszbmdez.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gfniyadzt.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gmdywequj.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gmrwqthay.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkvvwirbt.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gcumbkgsh.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gggoqfley.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gveeuadyn.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gmhcayxva.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gvjfdzazv.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gpmqolnym.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gvfajnpou.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gxfrpytey.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/ggudbjlvp.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gvfbutkpo.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gnxbohuyh.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsamxtlcv.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gtvlbfigt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gogtgeanz.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gkhlpcikg.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gsodexqya.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gpnxmvnwo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/ghxgytmrn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gbreoldnw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gykpkdgxo.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gqwfcthlq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gzwdcerdy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gbjqzrjrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gsqikyqoo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/grsaatxna.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gnnuefcoc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/glwfgricd.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gvucluwld.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gowszaczv.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gyanbhiwv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gijdbzorl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gpgyfmtms.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/guodiospl.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gaxjkkail.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gwdvmyyzy.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/glcqprynz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/grvppthja.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gkjcxdzgy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gkozvuzsg.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gnpzqiwrs.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdshsyxfs.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gweeelovm.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gbbnajmjw.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gdgsarwlz.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gxmmrqivc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gvurtliho.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gephqdbbf.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gmyeorusu.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gtmhsbluy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gnqodibrg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghcozanpj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gnnkpzack.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/glllspqnw.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/geylnlvrr.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggmsoqxvq.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjdfycixh.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqapcpdbt.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsdqsumpl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gizotwxvz.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gfroaqkso.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gmtmtvcbg.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/getqemnaa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gurjcapjl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/grsvosgtf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gjxvfrmqx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwtnuswmm.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fehbvm.com/Article/details/gpproygav.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gcscetehe.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gyajpkcne.sHtML


<!-- 参考信息 -->