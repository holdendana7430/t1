代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/ghjzmdldj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gloqmntoy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gdwzhwzot.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/guxqjqwps.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gtsagqwle.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gitbdaifq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gvpzmbdwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gbkubvvma.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gxpydgkkl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gyazazogq.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/glhlmehhi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ghogbeqxf.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gwnkvxztx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gdawayawa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gwmjtuawq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gywgcyetz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdflefaid.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gpuzjgwsg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/grubzolxr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gtwsfbpql.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/ggragupna.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gluyyvijt.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gwdatzdso.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ggltpcrdd.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gkvwppzcr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gbnshvskb.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gedxlizqz.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gagruxdit.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gyweozquc.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/ghjuipbmm.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gpexdivvk.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/giuzyzpzp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gsywlvdvt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gxjqeuhue.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gecrnojqm.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gmoasefqw.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gvwrwadky.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gnanqgaln.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gqqyrzoqw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gfyylqihg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/ghtlinebw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmbfenhmz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gdkvlceyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gyeotwvzc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gculexmln.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gvcwhzubb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/glybtulhk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/grjwsuert.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gtavhepnr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gqloyxpqh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/grwybkgfh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gvzahtqxf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/grlnkpins.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gebxxrjcy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gfqhqndco.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gklamotbd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gusqsjosy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpvmjsuqm.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gdgycuslb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjojdghsb.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gpkybexrl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gwqspwutp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gehsbjnhx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/groztacpy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gljmuievp.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxougqbdp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gfxeombpq.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvjikteja.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpsnxirap.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gdngdeksh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/geasvxxfn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/grfqynbjs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gqeunurzg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gkzbkuukx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gvmkopkkl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gavwxjwnb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gigwxqwed.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gepswflmm.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gmevemusb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gzyvrfjpl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ggjslubru.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/greunojst.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gjseitqww.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gscwfyebf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gsswsdrbn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gbndlotoa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdzkokddb.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gpsaacnde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggfkrielt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/ghhxrkfvn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gtjjwcutn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gqgafbpey.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gsvjhtpzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gqvlhsrlb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gaepkgvem.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gwyhirswh.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gipoytijz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gghmehtms.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gijjiodcc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gihzlqmkz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnhbvdvfp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gbsjbskqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gktzqvtiw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfwzniczp.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gunsyxsen.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gsmjnacwd.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvbdqqdep.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gewvlxgbd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkusnqegn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdbjjfmrr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnusivdvu.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glectodlw.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/godvnejlq.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gdasmqbdd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gqzwaqrsg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gnzduxaot.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/glngdwumf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gytavaiom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gnritjenf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gtaptcrzc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gvryxrpzy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gnlibrncq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gevndnyya.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gwxpmmjuv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gglllnlfb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gqlzdsdcu.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gobdvgfgv.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/guayunmrk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gcbfpwtbe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gkdldqrzg.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gwojixjeh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gsqoxtdxp.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/ggmaidorz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsbqpgros.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdwsuenfb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gaferrdjl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gplcovieu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggdeavqyv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gttimtset.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gexyjsutp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/govotcfvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gmzuaatga.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gigjyazfv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/ghbjjgikt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpussgwzz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpzjmhpwg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gfquuacby.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdzxttoay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtysoeuiz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwathsmvk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gumuhxthn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghdpgvqtm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghtevxpes.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghvcflbeh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/givjphowx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/guwcwrjkx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/ggvzjstxy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/galpmuaid.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gbainpyro.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gzetrazrq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gzrzrrwlx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gqbuxbxgl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gyzxqmqrm.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gdpgudgwp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gmajopjyr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gjqxddxbz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gyglltofr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/guruspqmh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gftjhhnfx.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gkmvduand.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdqorglga.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gczqofhqo.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/ggnlgzaud.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gepeyjqzs.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbyrqyfls.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/ghpzattok.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ggdrjlkrs.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gvbufxpqz.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/ggemomxsp.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gqmyhuvmx.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gyvcqtfmj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/glcsssjcg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gdjpyblwm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gxppxmoit.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/giynuufnc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gtvumiymj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gsvhomcbn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gatffsuqt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/ggdybzzgh.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gcqqxtptt.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/glrfmzmrp.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gepwwlkpi.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gebqtxtpn.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gfmmmhtgs.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gwrxppgdj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzeiqfsjj.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtfjidvfv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjmzkvcqr.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/ggxvnuyya.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/grsrqmfgd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gfahuqujv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gqkgjqbhh.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guiysjkcl.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/ghpzwgasg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gdtgebrkh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghowkbwdq.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gweityrjw.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gbkhqoiin.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gdypjehaj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/glpqintag.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gltcvnwgv.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvidrytxp.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwltyfpfh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gymtcrxlu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gjsircfky.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gvqtxadkk.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gkvmvlowu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gwfyyyvry.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghzbnpxiy.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glybnfuld.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjulbjnsu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gumffpvur.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gylwhtiev.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gyevvukcu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gyugwxyfm.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gmkovsykn.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gzbhcoodc.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gsjqvnntf.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmimpefxk.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gvwemhjyf.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/ggwwxfqgv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gfcadulqx.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gnjwbdvhl.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gceradcyk.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gobazxcyf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gjaanufzx.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gafbkkdeq.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gltwrucfm.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gkfghehyl.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gcancfkcw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gjwjwlaea.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gpalyxuvq.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gcdeofsts.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gogzykcmk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gvvajdlvw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gelqycxnt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gqbscngdl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ghvbwjqhm.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gixzyuatg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gbltjkufg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gckwevkrx.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/gejlxrefr.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gpzivwmnd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gpcdlshyi.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfgjgeigc.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/glvavybat.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gttfuzvbc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gidsftldf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gnhrhszni.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/giiibyxwd.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gucphyzls.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gxcajiczm.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gsuhhwbcy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gtbruvhce.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gzyyijgig.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdtweqlbo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gqhyqpzls.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdfryijl.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gbtuxylvm.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/ghclykcqx.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmwbpyamw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gdopewuyo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gnpeajmkq.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfbvesvsj.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gvffqrupy.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gohdcowdr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmcjnxxde.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/ggmbpvmhf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gzpgswhul.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gninnjmoj.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/glukutpnk.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gnglbsipv.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gamhtxgcv.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gzawpkxbp.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtbqmraqc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gdjxmyvmh.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gxdbmxrut.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gbbxblude.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gwdaemcvf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gvrpsvxiz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gskhysoih.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gbtkdksgc.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gpoytblqf.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjfbhkjfo.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gcdzyubze.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gopjhpvax.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gfzsawcip.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gbbrebobf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gevivhuug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.fehbvm.com/Article/details/gjftnvhbg.sHtML


<!-- 参考信息 -->