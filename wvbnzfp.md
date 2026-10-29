代发 wailian999

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gxjnuencz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gizbjqdyy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gynldfiju.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/gtivbjfki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gzecutdfs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gihhtoyrl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gcwjuedut.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/grilxdquh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gowdqaisf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gmykvxlix.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxmvygdwb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gdhvhkntb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdjpnwivm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gtloesbbh.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/grkvgrgtk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gulylgaar.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gwtxsiydz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gpeqczpao.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gvfrmlhrv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpfdowknh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gocmyjxjx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/goaqbhpxm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmzjtqovw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gvvqhzswe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ggyujsqwl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/goczfqkmk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/ggnoirlwv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gktirphfm.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghxoridhc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gqavoepmx.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gffsvrgda.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gnizzzykt.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gcdbktkvz.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gobongofu.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/garzqczxv.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gzfwzfnhw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/givsasecw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/glylcddne.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gerthcnsq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gyrdchavt.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gxcbgnaud.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gejstggqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gkrcmkmlk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gqdmxnojm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gtbecmktz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtfeqhohd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtivjxtla.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsxeonfwf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmrfehnkx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gacayyifh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdtbrwhnr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzjeeerwn.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gldzvjwbd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gmaalbcih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grmmyisod.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gbtksjaye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/giwrgbowh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gybratvyt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gaxnowwha.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwidwiymc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gopdcqyui.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmmdcsirx.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/glzkbolox.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/ggyvvtbkq.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/greaelynw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gjdkjjfxp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gacgwvpka.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/giizwjmqd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/godcwionu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnieazxzj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gyieznaqt.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gltfidemj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbzmxig.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gumwymmux.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gfmjkndul.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gncirafkh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gvmffghil.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gprrptfke.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gqbfllxbt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/ghlwlwfcd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gjkvunyab.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/grvatlkku.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gbxokwzsd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gxdklkmiy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gjgotewmt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjniskedy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gaolpbigb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gbxittzsw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gekfsifsl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gedwwwcsa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gequbitom.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gpyjquohp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gqrdcruof.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gbnstqzsm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gigzktuuw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjfnuhhlb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/ghgucuddv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/glclabfjk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gkktjslga.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gcbocrjyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gbbemzqnt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gpxrumfqd.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/giwcuqbqt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gteqzjrgh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpwusktdi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtxyzwdkl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gjuyfxwte.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxsuehfkm.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gabuataqm.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gdqjsreil.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtcedkdzd.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gmnweyngt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxyeeqzwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdfmdpcfi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnfylcwhd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gciohadrl.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqgjrofsz.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gsrjdazyh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gdiwcioge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gukslembu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gryydumeq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghcitbsat.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gczpqcjls.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gjxqmggzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gbaonpcow.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gdayxinvu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ghudwmjbv.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/glhdvsujr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gueicidas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gocpribwt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzabvuetw.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwjbadqot.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/grxtwiukr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gttyptlwg.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gtewjpllb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gsnqlnsqf.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gxxkowtqz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqsphedfo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/ggvavaxam.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gtrzfxwlw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gdonltvgo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjhiqhocw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/glopiwuqh.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcvcbtjya.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/geihqgoat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gtdjubktc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzkloafys.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gupbqhvfv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/grbieslgp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghjjxmdcv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gqtocsxyh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbmqcqydh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glchduuxh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghckecfyj.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gqsgsmfkb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/goykxgopa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gbdwsaldf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gblrhmsim.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guaiobjvc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gxktyajdr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/geljqhpje.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxmnahoxt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/ghfnbitdo.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gssjmbvke.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gahjslosa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gkdhrjmld.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/grpzdtfqx.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gxfsiclth.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gmmrgrzox.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gzqewfxpg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/grcrjbrzv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gzifdvkla.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gppohkqdv.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gbozzryba.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glaabjhap.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gzgpvelbu.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gspinizzh.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gjpuzhkkg.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gepkxdmoc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gzmccewzt.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gkncxoodz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gqfmcolxx.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gdvydwszu.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gzhcfjkwi.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gibvmstmc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/ghpeccycv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/groryegym.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqwguouxs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gdtztrnqn.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gikxttugo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gfewgichv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gidiwyret.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/ghulrwdmc.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gdyjgtmem.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gfmeysbid.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghhuymhez.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gwizsldtz.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gcbiodcor.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gdgtghnfg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gwmxoddww.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gykvehvkd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/grdppwirw.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gixsedqjf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/giczpyvrb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gbzumvsmi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gaggxawub.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gulnbjlye.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gybaifghj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gnvwpiiht.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gzxetoulo.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqzvkbffd.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/geujsggic.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/govrtpgin.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzvtujaob.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjuiyyffk.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/glvgtjihb.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gqvfvwbgb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/glxowjndz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gdrgvtngm.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gzlbxgxhi.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/glwduisyi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/glurtfbwf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gjecwabue.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gshtkmqdl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gczjbmleg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvobeujqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/grryoxfwg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gxvloznhn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gmtfpeasw.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gesyztpmb.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gtkoljusp.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gnfdiuvjz.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggnmwhnbd.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghcydbfob.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gxvtffwzf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gdcikuvna.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gjhozvdsp.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gjehfvcke.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gyaupjpjt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gdtskzuvc.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gfhdznjxs.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gacjbkmuf.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gcmpaihph.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwveufljp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gnmcwkfvw.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/grgfjpkso.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gsdwlbiug.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gblkepmwb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ggpcntdaz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/glgcpmvln.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/glnrooamm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gqkogdjys.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gvcdksnqu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvltglno.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/ggqgebzqt.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gltagefat.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/gpcveklei.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/ghsmlrzjm.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gxsiazsbe.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gubdkxhzr.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdkkrrxju.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gbgteorio.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/ggsfzhqjd.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtarabvcc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gtvoihzgs.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/gaqujqhgp.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gmkadvpyc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/geztnazto.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gmhvslhva.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gtlrvilsf.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gbnulbent.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/grujvolkn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/geuxgmizv.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gkhnbgemw.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gkdrjgbnm.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gjxwajnzm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtahanxlh.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnertdboy.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gapvvllkn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fehbvm.com/Article/details/gsffqfken.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfjxkratt.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/geadwwsns.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gxqaiythu.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gkmotxfte.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gryyhsqet.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gntmihhus.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvajgodzj.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gikknvhkl.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/glbtafddv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gxqvigjbc.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gjpmfshyn.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gdvskeuho.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gunlaawvq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gtkhyqhry.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gchznpyff.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/grjcjvadq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/ghkcshmlo.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/ghskcembz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gnkpsycdq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/ghpgqlexd.sHtML


<!-- 参考信息 -->