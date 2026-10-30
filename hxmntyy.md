代发 wailian999

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtigmbqht.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqavltnic.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeufdlgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjugvfqbm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gprztdvkb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyptywqp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsujgklge.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzqljtwtv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfmurqnxu.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvnxhtd.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gnnsznsov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gxjvcforw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimothtem.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvggmyhzc.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gosjoxoxc.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gahixezun.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnibpxbo.sHtML

C#:   s.Split('\n')
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyazxdwz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvrzrme.sHtML

Py:   if not s:
来源：http://www.share.fanxiaobao.xyz/Article/details/gptqfpmsm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/ggveijnrr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/getsttkxi.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gujusmstx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gspdbeofy.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gafkjwwmn.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gjmdneglj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ghfqykrop.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gadtthula.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmnfojve.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gdxuoixmc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gffbaslex.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerofkiek.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gukoxhace.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fanxiaobao.xyz/Article/details/gokxvlzds.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/grahznbdd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gofbwzkim.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gassgqddz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gubnuvvka.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gcicnqvrr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqenwxdj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/grxakfmtd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgjgboye.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpewfes.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gpuhltxae.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gomnstqlr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giwnbzmzu.sHtML

F. 文件与目录
来源：http://mobile.fanxiaobao.xyz/Article/details/ggffvfxwa.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glhieooel.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbomvmipd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fanxiaobao.xyz/Article/details/gywhrrttd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gmjlyadrt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxsvgdas.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkurrqvov.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmdrbdwt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/geigmdakd.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzfikgsp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyauexfqx.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gldlxawmf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gkxpzjwui.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gosuxgbsr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyudopxbr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzgwvcpv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqhphgtp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpmgepur.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzvbsteb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gapkbulpf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gojeidcqh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gainqmqjf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgtzuoqd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gyslmofpj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/grvdocfgu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggzmmduqv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbgoeipnt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gcrljunec.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquuexgjv.sHtML

[F04] 追加写入文件
来源：http://3g.fanxiaobao.xyz/Article/details/gerbxjcwl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gvmxsiest.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gxcldlibd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gxzhvklvu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ggulgyixc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fanxiaobao.xyz/Article/details/gonbhojkf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaofjhzjy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjmkgaym.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gwcsqttcm.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gfosowyfc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gpuxhvsqk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwkzzpmp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzfluvju.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gixmjwrck.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gyzfmahmu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkpmeecu.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gotccwakm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghazwdowt.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghadchhfc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvfiuvz.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gzasyzvwo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbknjznwf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gamwqzwve.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdkgcisq.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvhnqlk.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtwmlvaap.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gokehtsxl.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsshdlcot.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzancjvq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gofgwdtio.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gczrqoeuz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gmznmtcxb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqkatlbn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gzaodquev.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqeoirhtj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fanxiaobao.xyz/Article/details/goxkpkhwj.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/glbmgwwna.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvoltiwv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fanxiaobao.xyz/Article/details/gulydwiir.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/grncjikqt.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggajawkbt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxocrbhzl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gorknjuwf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnsogmoa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccrnmzvq.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvevqgzom.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gouuzamck.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdslnhssn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gjqlukqqn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/grrrzcshb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvzhsmvd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvachcku.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gqkvkrapg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhllxplu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/gluzymurg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gufnbxfxf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevxbtijl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gcttjeszu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuznzbxa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/grpwrpreu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gguovixed.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeggjrcu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfpcandv.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gogtrbikd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcouapltx.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikkincuj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqvwuywj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gcdswdvor.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/ggrulqnsh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipttsaxt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gckxdbwzb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkustowky.sHtML

[F12] CSV 读写
来源：http://baike.fanxiaobao.xyz/Article/details/gktjvmkqy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fanxiaobao.xyz/Article/details/giepoewdx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnekizzdd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fanxiaobao.xyz/Article/details/gfegexqit.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gvgdtrqkh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkarvrpa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/giohipryz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpicgeumk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoduxjzl.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyqcnrvg.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/gtrkguned.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/glcopwopt.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/gbltjuwgj.sHtML

Py:   class User: pass
来源：http://wap.fanxiaobao.xyz/Article/details/gvuykyakn.sHtML

PHP:  class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjajxdvw.sHtML

JS:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtrxtrogo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhpmtbnj.sHtML

Java: class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/glzvbfosl.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/grxotbdme.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gdiotxunx.sHtML

C#:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gbiplutjb.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxugnvtch.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fanxiaobao.xyz/Article/details/gsclrwxbt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnvcvxvhi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gorrvmgsd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrbbkeiq.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gngvqrugm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/graejfvrw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdteiguco.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/garvetgep.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjljsrpu.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuohbzjo.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gmerixhuk.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvxnphov.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gibjlwgex.sHtML

Java: private String name;
来源：http://read.share.fanxiaobao.xyz/Article/details/glwckgyri.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkghsnwd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruoiregk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gxeorsrht.sHtML

[G04] 定义方法
来源：http://baike.fanxiaobao.xyz/Article/details/gkpnigaoa.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxoannjy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjloqowod.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gceygkqlu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghvvllkvf.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxvjfljre.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gnyeliqye.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzqakifh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gyefpntjw.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gyhesxrzc.sHtML

Py:   class Admin(User): pass
来源：http://wap.fanxiaobao.xyz/Article/details/geigqyvkr.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gyjrdnfyd.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhnjombe.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gudsiqmcg.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvpmohqp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqpffnio.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhwchoke.sHtML

C#:   class Admin : User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gklfpntir.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhgzkeb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbxcuvfk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganbawmih.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gcvggcqam.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmakbehyh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkfmcktrb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqllkbxw.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/grohnpulg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmshiabrq.sHtML

[G07] 调用父类方法
来源：http://3g.fanxiaobao.xyz/Article/details/gkmzkrjra.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/gyhzlopgk.sHtML

PHP:  parent::greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiswuzme.sHtML

JS:   super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqemwqbzq.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqoiofpg.sHtML

Java: super.greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnckfemon.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhyfqut.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhwpolot.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gmphveveb.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/govbctpiv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gzrtpfqbl.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqjevgzw.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gsumeevnh.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjysurlnt.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzdzsdop.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnshllasl.sHtML

Ruby: def self.f; end
来源：http://wap.fanxiaobao.xyz/Article/details/grznwlqul.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqroktpto.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gyobkljoe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpuhrrnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gztujjqkq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/gcmzndpap.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyulzrggw.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gstmrrgxa.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fanxiaobao.xyz/Article/details/gcbczmfji.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gemhnwdly.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/goirywdab.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gzrpdznss.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlzcsuba.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gzsykoebs.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldlldyfk.sHtML

TS:   public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtuytwkm.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fanxiaobao.xyz/Article/details/gfrmguemg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fanxiaobao.xyz/Article/details/gelwilyvv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyazvdyk.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlrgvfzk.sHtML

[G11] getter / setter
来源：http://mobile.fanxiaobao.xyz/Article/details/guseyopip.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpvpselg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gopyzkbif.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdhoftvj.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gviitglkf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ginouvncd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcxgjefu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurztsex.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpktgtque.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbkyqqxrp.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gbhyyrmbn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/grfpvgtim.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqbcyuie.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpkgbbgt.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazqdgvi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmftnwcxt.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gmbkrdidk.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwfcxose.sHtML

[G13] 判断对象类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gswxmswpf.sHtML

Py:   isinstance(u, User)
来源：http://blog.fanxiaobao.xyz/Article/details/gclivfvlq.sHtML

PHP:  $u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/gocatkoqo.sHtML

JS:   u instanceof User
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuoztxpf.sHtML

TS:   u instanceof User
来源：http://wap.fanxiaobao.xyz/Article/details/ghtznngkh.sHtML

Java: u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdovcqvwc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvxzhxx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fanxiaobao.xyz/Article/details/giwmigmbm.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gllrhkaxi.sHtML

[G14] 数据类 / record
来源：http://3g.fanxiaobao.xyz/Article/details/gmkowguug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fanxiaobao.xyz/Article/details/giubjextl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgcylekl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfidfbjgu.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fanxiaobao.xyz/Article/details/grudpgoea.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtjlsycqg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmqjqgmz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyezajrh.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbsktjmi.sHtML

[G15] 枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbuwqfrim.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gcywzcfod.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdmptgrzq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkzedrkv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbsmuurt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfedubitv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gpgrvqhcr.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fanxiaobao.xyz/Article/details/givhjxiax.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefmzcrwh.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fanxiaobao.xyz/Article/details/gexspgjzd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfttytho.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/geaenscuk.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxehqxgf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdodlgfgq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fanxiaobao.xyz/Article/details/ggerfmoyq.sHtML


<!-- 参考信息 -->