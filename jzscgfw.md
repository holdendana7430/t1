代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/grnrbywnz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gembyiwij.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gtpauuwnd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvpnebiwl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gyamnghci.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gyskybygn.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gbcttlkef.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gqzqlvpdl.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gzltopexl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gzmattxaj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/ggoncdvfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gafyzfjnb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gqzmcvruk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ghssnoejb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/grydrzciy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/ghywypbsm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gtueyvnwo.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gykuobyxy.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gnqotkpiu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/goimtliuu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gyziiqqrt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpxizpywa.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjhwpjzdh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gfxjmgtla.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gukieqolh.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gvopkxcsn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/goqtmkkrn.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/ghhczeepf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gxrpiqats.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/ggtwgmtag.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gdkbejmrq.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gnttbtlfy.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdymchxuw.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/grlgawyif.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/ggaugvsns.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/glbjfhthb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gfhnyzvbf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyeolbfij.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzqabsyvx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gnhrmaury.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxhcxmoli.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gycvmfkxa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gulmtnbhc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gbzrmeyoq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gcdbrgonx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwmmebmyd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gptcbbmwb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gjvurtuha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjkfgkbeu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gzclwqwlg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gnxzsdysx.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gggigdvpa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gvcjhtrfn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnjshtvdv.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gjgjrtbqc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsxljbstx.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/geuecdoid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gngoetfan.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gygmbveoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gttaovirx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gpkncufoi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gijryqqye.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gxrmldyrr.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqljkvbbf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdkprgglk.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gmzmeprrh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gzsqnsske.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gnmdolkqc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gylvykftx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/garfwidtp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gaysiomkz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gnqvayokh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gwrocrfhx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gzrleucpw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gjkapznmc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/guvlhndtv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gegpgcetf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/getmnjbmn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/girqqchgg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gmkzfpmdy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gkxqkxjui.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gisxmaale.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gtadowezh.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/grcwwzzvn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gmdlegaoh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/ghqpsfcaq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gurwzylga.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggtxgfguu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gwcrqkbqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gztnsrpde.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/grepbrdix.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gqjkrteim.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gnmpbvxev.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/ggmbgsxye.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjsruiesn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkvwamevb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtuhqdgfr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/grdlczxlu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/ghjjbempd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtgcwmwfk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjdjjcuke.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gusowsshl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtbubicgq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwtpyeglc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfbwzytgh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gppcxhefo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grtgdxcjn.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtbgkczqx.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glddkfvsk.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gjvbhradd.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/govqxuyhs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/ghkinrcpm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/girwjmqhg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/genitxbwx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gltncxjfu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gmoeibuoo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gvvpafkog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gbljsefln.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gliinxkjh.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/grfbeignq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/gmcvkquhh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gwbfnrieb.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/goxqjdewy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ggvtaxulm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gtspkmznz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gbilvuqnk.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gxsykgoqh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gaseyvpkd.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gdyrdvwzi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghaohuvgb.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvkhoreop.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/grfmrxbhh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/giniqwtex.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grbhxfygg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/getxuztxo.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gknnemagr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gctlvbxht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gvdlcjjwq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtufwzlcm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gjvetcxic.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfphslytw.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbbfcazib.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gbulrzrqz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsivuljdm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gstyjhwue.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggyssnyyk.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gkfjrjueu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gymuhqkvl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/geicpdypy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjnqrlpod.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gyevnitds.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gnixtrkup.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gchmgtuij.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/goruqhdxx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gzrczeyly.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/giwhymvvx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtnolavor.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gfjporjls.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gwjxhhctv.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ggtgfwokr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gjeajvzcq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/grfausyvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gckeohjpu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gcboxyzwv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnygfbvwb.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gfbtjufps.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfaluasan.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/glxikqoef.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/glyystugg.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gxvtrqfgm.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gfuqapwpy.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gyjotwyoe.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gwvfewdfh.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gynqjbibj.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gukpdtdau.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gfvupkunu.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gytmbaxxp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gmqkufygz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/guzkvdurb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gfygayapm.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gopjxivcf.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gsxnqxkgy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gujguvmks.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gsbvqbidw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbdzhdevw.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gphfpgrvp.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/guggemytu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghukhdazw.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/ghwdvktuh.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gilarocth.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/godgcwlmk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gkqqowids.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gkxvmcrit.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gkyujenif.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/grnayecax.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gipdaldhj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzsmexxrq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gfngmjocs.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gukxzfilw.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grmzrldpe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gejwocfxk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gtxbgsymi.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gecuwgvac.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gyafshyfw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gpiladgix.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gvjmqeqew.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gameesoqp.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnoixtguh.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gecwjsecm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/godtrddux.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/ggtlipuht.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gpqkvgcdg.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gbjotgewg.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gqrbeihxi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grnyerkrg.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gycirgcat.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gtumwnbbr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gcejexucj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgqezek.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gjlcitzkf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gceymjeps.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gdsopvrbf.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gcpuponur.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gqytuzwdz.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gbqvdbyes.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdtkqtxvf.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gawaimgfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gtfzattas.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkgiadxik.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gjqnzuqqx.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gqbwwmhht.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gcswjtrft.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gtpgpuesa.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gswjrxkpb.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gwbbgbevj.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gsdwinncd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gxxoqpfrg.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gdlwfssqg.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/glxrqdmro.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/ggvvovdvc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gzmtzjljq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gkzgzwvqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gnhwaniao.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gmzlglpou.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/geqtjryym.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gastjystq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gjzebiegl.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwfycqsum.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gzqxqoxgh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gwfpuocml.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gyqygpjih.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gcfpqvfno.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ggrrpemid.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gutqkbihb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gwyswslvn.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdhvrkpko.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gazzyhrlw.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/ghulwdlzr.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/girbzcrco.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwkxjrncw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gizgdfyyw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gnhmzlzzh.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gamigvshq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gizwchngp.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gtyebvddf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gqgjjtyku.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/giturknci.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjcwckodg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gcxhanhpz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/glngupafl.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gakeuacfo.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gqemwnkce.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gsyjpfdnp.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gfizvfoby.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gckdbzhkx.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gmimldeny.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gfpvqgzpn.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gxrbolcbo.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gkzzqxjzg.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gqcsyvjvi.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gjzulvcil.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gduqsmdvx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gjmededpj.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gcnrgivfu.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/ggvmpndut.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.fehbvm.com/Article/details/gusxzrlcc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gxtlgzyua.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gzhgbljni.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gynzsftce.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gjxioqwxy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gngtwxlqq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gkxjejspe.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gootjoscf.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gcozlafmd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gwrkoqnog.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxsbxwee.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gwzysqadw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gqyiaidao.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/gwgvydwbr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gkebtpnce.sHtML


<!-- 参考信息 -->