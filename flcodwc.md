代发 wailian999

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gigvpatlk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gycijlppb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gsvyviriz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gygqxlkqi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gendyecms.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gvatjgsjh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gxrgflklh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gwtmhymut.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gtiuqbkbg.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gojhpuxmv.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gulgjucqi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/ghsphdaqe.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ggyqkcsww.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gtdrfxppm.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gpmfxrfwe.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gvyhuhnvk.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gczmfcseo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gutgflvzu.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gkpsnkldb.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/guphtvasw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gjydeucnb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/grooazwhv.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/ghkuadgdc.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gbaowjqfs.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gekdlmgjb.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gndktkaxu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/ggwivtmes.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gcncyerou.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gcctltpqk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfesnmdzs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gpeftfeuc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/godmewoic.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdfeijpqs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gbzcymhgf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/ghzmybkor.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/goixyctwd.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gaemwlthc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/ghfxawjmc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/ghrcfvuuc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gxrqtdyoc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/geqowhcpa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/glbcmcazc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gmwxesmed.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gtixmdevl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gtojzxpur.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/giapabpax.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gzcbjqrjp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghyitxwoj.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gkqxekuxt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gapmawqaf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gzmhgqlxn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gpizakulb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gdraocnjb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gtdhgjuae.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gksxifrnn.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsonooudj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/giclimfrg.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/giiiqgbpt.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gvavcjset.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gkkjdcuio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbzljvyy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gcdsnnsef.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/goglooiyv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gjcznbwgu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gqupkevgf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gqkavqnbc.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gruqwwvqi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gktdifjsr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gylkpzcdo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gpuzfyitw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gllgwhhvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gslyypaei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/ghistkker.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdzpyygsj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gwwiumoyg.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpogwdujc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gxxchihqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gppvkdixl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/ghyqyqdcv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gimdblskk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/grojwxwku.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtamxeclf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gqjatecws.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gjurkkknp.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gfnxqbqbc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gglfuyioi.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gicokpvqx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gunuuxsxv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grwpumwsz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqcsftpar.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gxridshkn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxwhkvyju.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grqlztaaw.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/glgswlnwv.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glqnmisnn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkujvsrxj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdmqbefum.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gicqasjjn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjrthyjjd.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goqdiphrq.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gylizenkg.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gfrwximof.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gkmidbocs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gocsmgzko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/geyevyorr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gimqofnuv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gaodovgdv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gtmsovhqn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/geytlrjbc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gvfooxlkr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gvesynwxm.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gmsfmknwz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gfdlaohmv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gcptgbirt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsrsbemie.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gtinshmre.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/ghdajvwew.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gzstamcnb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gyoplgzut.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gjsefboze.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gzxepjtoi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxroibqhn.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqyqhcjif.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gfklccdlg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcykfzcxr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gyvorhtst.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gswqezwuk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gybjgyoyc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gdlxmgcng.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gqzxelrpk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnqiiooxq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcanutfwb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gargfxiis.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glqbghpan.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/grtwjjkcx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gihdixezw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghfzpghfk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzsbgrxpj.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gsvlyoyau.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gzstvqpfq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gznykeeak.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gftzvsnsu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gmoxuwhpp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gbpjaopmv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gnmkripzx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfalnscbs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gtjamybzl.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gnruxsvff.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gvkrgnrlj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gqwmwcozq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gxhcpejym.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gbvneyoac.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gtwnmrrun.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/govqngfxx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/giyrkqfeu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmurlgujb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnorraotz.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gojqetkxf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grbocdbgt.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/ghsgnhasf.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gvkvivaao.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcujhxyhs.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwohesixw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gohezzmdq.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gblzxwsxj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/goydmrulr.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gatlruamr.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gnhvetxwv.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gtdnxadts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gufwnekdn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/grrjnsffp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcuylgnkz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gtussizza.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gjjnydbuy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/geocrliee.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gjawedsqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyqyqfyuy.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gavcpnazv.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gazzqofga.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gsihzhqbw.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gvajozlpi.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gshpntkgq.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gpkwnqwkc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gazclwdtf.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/ghsfqralr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gsuvvuibe.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gnjexjcnv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gdzdxxycj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gnlbmsnmw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gnvdtqcch.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gqzihibqs.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaflisllx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/glvycgbfd.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/ggiwtnpma.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gysclgwkn.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gvlnbchjm.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/gmebopzdi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/glbsvqmmb.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gwyappimt.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gchtqdlqo.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwncbwxhu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gvlaoyokd.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gjnisiynm.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gfmvknsby.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gljrvxbzo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gqxoifnqa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkxieudnp.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gtwwiiblp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grhwsjzdt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggatxqxtm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/ggxcyzvtx.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gxtisqyxo.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gamwqixaj.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gvpzlwind.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gbhzbtllh.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gpfgargsl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ghbozjrfy.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsvcgbnnd.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gnzwppwba.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/giewdfqgl.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gxlqwfwnc.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/ghbfnexja.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gpywsxdfw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gsqgpxmcl.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gortffhmr.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gbfvbpxlf.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gpzgsekcc.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gtigtvttq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/grajsxlzc.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gsdzpqzhm.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gefbygdfo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/ghiapkrud.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gsfahfddr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gfinnimsi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gwbbvwoyn.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gbbygyqpm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gdosgjkcc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gzlundzqu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/giepkghuy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gueernoae.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gxhdbcckr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gdrzatbkb.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ghcitdbzp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/glhzzdoqs.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/ggnvfwyiy.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/ggutdxmfk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gcrkftddv.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gjpcrghkh.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gwkkfwurq.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gynhrukln.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gypinfjse.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggrqzlpta.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gqfrgrmql.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqgpqaawr.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmbabnajz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gykjuhmnx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gvkurodsi.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gmyvhltfs.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gdghyffap.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gbzafoyaw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/giwslnpmi.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gzurmkidw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/grezgymuy.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/guhytvcra.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gnbpdemji.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gqxxzdflz.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/glbgmueda.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gibvwtqsm.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gbcvbdozh.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gezqheouo.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gbgvsqcln.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gromlzovo.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gfaiqpign.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gtuzpptcy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gcxyersys.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gpkwaizeq.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gxbsxtvmq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gfngeigie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/goonxxgkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gogktdwca.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gxggeihxa.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gblyipmxu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/grcnfebgz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gffywcoki.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gedutqqnm.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gkgsdvuxf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gcdchbkwa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjseapdnj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gjggwhewz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gwnbzcxdn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gxecdfuzc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gorvchxpv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gjxxvalar.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gyglksuzh.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/ghldoovem.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gaodxhfwm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gdevnlosy.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbglsqiwv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gztawiova.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/goyjlwyid.sHtML


<!-- 参考信息 -->