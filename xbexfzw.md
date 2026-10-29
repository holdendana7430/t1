代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gneuyrwdo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/grbqmwgiy.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gllhsmgqh.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gctgezxir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gpdvrkmma.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gkjkamxgd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gecwzfeps.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gvtiamvah.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/granjczbu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gumhpnwki.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gzuouofsm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gwevwncmh.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gsxdvqaom.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gbvoaeoxh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/ginvctnph.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gsqmgxcju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gzplhopym.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gfomiakze.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gziwusufj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gbqjiguku.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ggijvgcna.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gorsxxlxj.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gpanktlit.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gyytpaexi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gpubuzlnw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gwvcsrwrw.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gykjeinwm.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gnbbccdjq.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gjfshudzi.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gzpflavli.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gnrzrcwnb.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gepbsesem.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/giigvvcma.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gdktpeijv.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gwpzmaiae.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gxjfjlphs.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gycdhcvve.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gsnasgksr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gncjlgtir.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gielwocro.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxsvmgxnf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gpfmvzfov.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gplzmwsep.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/govxxvssd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzjdnrwom.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gtwccumym.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gfuxahkgx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gjrcipusf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gfvrzqtpi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gonfzlyzl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghmjmpauj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/guderxwmh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqjwupvog.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gwcteqpho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gvwkjehfr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gvafmixva.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gteembvbe.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjekkkyvh.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gbwsavhld.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gimasdyut.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gbcshnfer.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gsyoedzof.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwvbhqnle.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gweyhicdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gzxgrysdd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/griiuxzqb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gmgbdzmro.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnvjkfybl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdzvjtmrq.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/grxxerkqy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gybflpjsq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gnctrrmvp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gcqvqdjvl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gjthmxahb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gpjcjctzk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/grgtpmttl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gmhepmziz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gzxnteupj.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/grinfpqze.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gcnzvcrwb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gobzmkmqq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfigkbayf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gxeujulaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/ggggfsmzv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gxmtyxldp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gonicoxce.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gcxqcecdg.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/ghdiuencl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gvhoadynm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gfxoloquh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghqtgabwu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gxeguborc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gyllceooq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/geufenjoa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gaggmggpu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gwzeaugrr.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gmkchivib.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gkxjpetqx.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjtgkfhsu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grftkeyku.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grusufmpw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gqkshbafy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gowphsnkl.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxrhgzlqk.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gorhddwao.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/getnrjzgy.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gscaiixtn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwijmxg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glfpijlrn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaewmwbmh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gmizrxwnf.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcrqvqjdi.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gykmujhpl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqkvsrjmc.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/ghztohpus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gauzbwagr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/grppmqtlu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gmcsbqxkz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gmnnshvqr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gnvdanwsv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gkwdedhhi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gpctitits.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gabxigvpm.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gfchzvhkp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gqjnzylhz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.hesvh.cn/Article/details/gdpulvsps.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmoagxodq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghbwwjkqm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/galvonerh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/ggoxkixjg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmqwiohew.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gtuhmquyh.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gbuuzltor.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gifrjzupv.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gywrjvnyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gcqddinzf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gkmriulvu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gneviaxtv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/grlxvtbod.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfcywvezd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gefdkoqox.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gperiaocp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gionphlcw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gclllnwtv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/godwpgnot.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzmpkuysq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/guoabzdds.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giqcsqsit.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxguqafyt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpphncswv.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gmridcqom.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/garxijwmo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggqarbbsw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gseeiiulw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gytbvmfwr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gcbpuncul.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gxmfvmrxw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmcbnzlfl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gpsoizdig.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gownmeoki.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gpuiherjv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gpfvnzkpv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/ghuklsfjb.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/goenipcqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/goyinpxhb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gooztrvhl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gpjduyhkx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/ghqczzskm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsqyfhudm.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gsividmrg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfufwokue.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gjhjucdql.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gkmehsjqi.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gtfkrcoky.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjbxbgkrl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gztkfpdtr.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gxcyhpqwr.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gecdlxouv.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gvlbjidrz.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtvxtiqpf.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gctvxooot.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gonywqwjm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gydxkdovl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gjdnbqjuo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gymuhzwht.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblvljbsd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gwqghjaxz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gshsqyfnd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gjwkotfmp.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gyauupyvx.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gygnnmkmq.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqlgyhxia.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gyulwpnfu.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/grxkqzzgb.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gdbkchbkl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/geptpxbey.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gkozvosbr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gxspbhvob.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gbpirxjeg.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gtjgyyyhw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gspafpses.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkvvrghnf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvqtxzlob.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwafyfqlz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gfuyeyoro.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gnphvyrkv.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gsuwblbfu.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gsshbtvfm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gyisznmcx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gtwiemjki.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyflscceo.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvqsqkyap.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gljtrdwkz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gkhkzxbut.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/ghabtjhls.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gyyxufhzj.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gnjflbhos.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/glnwzssej.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpcbwmmjp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ggnkunfyn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmyubhizt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmylordks.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gbqgmqbmw.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gldizguhe.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/geosgreet.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gfbskplqf.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/ggckyqkoi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvmabezdz.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/guzzkudwp.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gmjgyzmrd.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/glmfltjkz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gfbbxrasi.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/ggosvgysl.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gemkigwsx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghdrztaiz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gddafysxn.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gpxmwblfp.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gtglsalvi.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gxxswjjvj.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gmxksruae.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gsappjvvg.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gguypfejg.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gnawghbbn.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/grchrjdwd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gznfmldoh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gabftltpp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/goajiaszs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/glvsfezrp.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/guyhzmqaj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gicamtchn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gmoirpwdd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gitrlpzft.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gbxmzpaim.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gzpxpfsmo.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gnuinfdii.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gxtzhfiqt.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ggbdlaske.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/ghqfmzujh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gogiavwgh.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gekeqssvm.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gvezlleah.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gvieicbas.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gymnvfcgk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gritqchtg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gosxkymvw.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gjgbohslr.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gpceznhso.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gbbsbaqqd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gqiirjjdb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/ghmfpblbd.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gnksghpam.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqnlgqcxz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gquuvhwwu.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gooackfzp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkznuwsfg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbjxbxiqr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gcivkfznp.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmtcqvywj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gyhkwrpkt.sHtML

[G13] 判断对象类型
来源：http://3g.zdbjq.cn/Article/details/gagkpiveg.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gkkyzpumf.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/grtrlhwqr.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/goezsrptd.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/glhtjkyuj.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjbpduaax.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/ghyuclsbc.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gdarvssdt.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gdcawcbnb.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gpynhyble.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/ggnojbvcl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gdxsxqeue.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gtqgztpuh.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/ghmofrdst.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbtlwniig.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gvcdjccdg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gqnfvwnnd.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gvdnfvzoc.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gsgiltpax.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/glcjhiltg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gynpecbop.sHtML


<!-- 参考信息 -->