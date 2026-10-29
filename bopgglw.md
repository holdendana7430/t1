代发 wailian999

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gfkbleemi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gwadmaece.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gbakluppt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwnbicvjq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gkkwedvty.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gbedpizvn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gisjrajry.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/grdttdhyc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gfiazjomc.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gwuckfbou.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gndjfjiji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqicvvkfp.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gyqszklvp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gibowgrip.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/grraewtyj.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gtecvpusv.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gxmgybsbi.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gmpiqqmqq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gilbguwtu.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/ghuksnihz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gvfdmeiri.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gixniebir.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gjgsaetod.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gcntdiylk.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gsrogkshh.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gkupsabtf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gbccxcbsb.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gpkkdbayt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gnytjunzn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gxjyjkjab.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gkhllusak.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gqopzznrq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gekyhkwqb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gqwuvprzd.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/grukphacy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvcchetxx.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gtvduiqqi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gtuxovxfd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsodcrofj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwjachobh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/guahaxopv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gotfqiocl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gipczteoo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwbbpgtvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gwijswuxf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdfnsmqee.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gcncgltql.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gruekwkch.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gzwsipwum.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gppsikurz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvezvujle.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gmpuoieaf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gcpfemspn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gsspgozdh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/glkpdaxdn.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gegrvzmjt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyffaadbu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gkjwkahjw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwlgloryk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ggeypzodd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/grhjiuaoo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gurvnmnom.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gfhdyycpf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.zdbjq.cn/Article/details/gbocydrdo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gzdrkljxu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/guifbqwjz.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gopdhssud.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gvcdidzlj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gjhejjdqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/guinmkqtd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwtghbswx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/grdgsqgak.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gonryebwn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gtpjiotcw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdktrbcbv.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ggqqrlsoc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjofukenm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gnjzrqeog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/guotvqyxs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gpgnanpfm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gsyoxstax.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gmgrlwjjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gobmqjixq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gbkexlule.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/ghazdxtoh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gpmidychp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gulqboorx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmceesudb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gylbfhdhq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gzddhxgwy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gwptxxyem.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfbbsguxu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghlujsqkf.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gwyylilkp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcjqjuabu.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmutqbswh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjlboaskc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gietsveue.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gizzozbve.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnrutpwnz.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmwlghkps.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkpeufkbt.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gjsmihuib.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/glpmymfnw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gwwrwrcvx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gwmbmednp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gdwtuwprs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gusvabunu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gqmiirfaw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/grywnlipv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gxppqazfe.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gginvvfpt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/guixaqjme.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gbdfdgmdz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzcbmefej.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gqraglfma.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfzuwzcxv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gjgxdrlnq.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gwsdtxkev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gxjktwuhx.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gxsudfnhn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/glbmeosai.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwovltmfq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gbcwpspvc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gpjapugst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcuzywgso.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gyypmuwjk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxpnixcak.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gjgjqlgyk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gjxwxpjaw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gldossmkk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghbvrbcdt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gnmqedfyl.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmycoogkw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gzpajejlg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqewvnbid.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gazdtvkst.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcpqtwwdt.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/glmuoabqn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtqefkesz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gyfktxlot.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvimsojck.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gourxctqj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/guufnlrqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gjbozpwpb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/giaclevbc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gfmdqaevm.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gfwtndzye.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gzxryritt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqyxnzg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gaphnweer.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gycflrmet.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gsmxxllhd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gbfbgxbcs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gtzqvnxpt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gzhlszhmi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnfsybmjx.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gwqwczckz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtnbsyfsj.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gouhaagqc.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gmizfcjtu.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gadoissap.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/geqvlwhvl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gezmrdadk.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtggumfar.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/ggoqrkefs.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gqhvzlxna.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gtmthtybe.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ghcofhfnf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/ggdvdqgah.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gimehiezv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gjchnvvos.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gvpgoiklq.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gfljjlimq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/geedqvbgx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/grtoqvsbh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gbmwrytef.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/gfehnmzma.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gaotrgugd.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/ggkalrpml.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/groqyhvzp.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gxsvanppn.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gigsxmmhe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gaqzknuvx.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gmfwptzqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/grlebobuy.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/ghgrhwhjh.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gajhyhyzz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvbuczjqh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnecopdcw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjxrolijt.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gljxdffww.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gprotjrhw.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gbliusoiw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/ghlwynvtm.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gpsslxdwh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gqdehevsh.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gdtcatced.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ggqwjvavt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsozyncya.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gallenrnf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gdfctdvly.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gsjhtdtkl.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gaunzxyqe.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gychbaafi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gdzovbpiw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/goqtmjjcf.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gaqlchwsk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gjaivavbr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/ghcvwnjny.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gurayoekc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gispithkn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gtvntpbps.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gcditxwkl.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gyenelfrx.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gjjtbvtef.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghxexjbfq.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/guvdiyhvm.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/goflmlfgr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gyrijzuhq.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gfqbqqkns.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gqwoaoraw.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gfzdnxghp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gvdppwvre.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggfptfang.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gubmfitye.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gmufutups.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/glneeqahd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gjwnebjdz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gmlrqvcfx.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gmoxrbmxp.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/giaqimnfb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/glmmfetej.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/giydyctvy.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gcsanvlft.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gnpknjmxk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gwbsdkunc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gyemyxjrc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/ggkuifwom.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdtbtbj.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gacjiqftk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gqoqshgyh.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gvtybjjbj.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gotogheec.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gsbrhciro.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/giidmbfai.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gslqecnoz.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gkfxjrlqg.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gxoarosrx.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gwsbtdlhi.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gqxakqowk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwjhtydpk.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gcecuibsi.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqebwdtnc.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gkihkvgdm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwvrzxuhy.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gbuygwxek.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gjweigqqu.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/glwfzoncg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gvasfgkos.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gqwesebpl.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gxqxnfhvt.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gqlrcgfpq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghjmuzyvk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gkykjunvz.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gcxtlinnx.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gtgsbgbsg.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gzpafvvhg.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gzyggefaf.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmcnhluay.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gufjpxgcg.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gscjxnyad.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwtvrnuuc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gbwytilpy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gpxzepnlw.sHtML

C#:   u is User
来源：http://m.share.fehbvm.com/Article/details/gbmrzuaex.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/ghoofnzsu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.zdbjq.cn/Article/details/gcorifaxb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.zdbjq.cn/Article/details/gucebarfu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gshshriol.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gxdhlkgrj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gsjdgdlmt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gkljjmnef.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.fehbvm.com/Article/details/gwfkamcfc.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.hesvh.cn/Article/details/gxwxkowre.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gknzvbtzh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gtmsbhkwq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/gayiusgdb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gbdfizbal.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gtjmkfwbd.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ghaivfrbo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gfnyqgmef.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/glkfmetpc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gdhvgtwzr.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gajepvxxp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gutllqulg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gufssdxzo.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gdtlsshsm.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/grywjmejh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gzomtdxgo.sHtML


<!-- 参考信息 -->