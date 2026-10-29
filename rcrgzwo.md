代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gqhpbrcep.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/ggoxuwwfe.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gpyfdpjtn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gnciokkst.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gxfbmernc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gwkthghaj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gwcqpjbsg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbingjevm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gelfmvkgu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gzujwottk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvzbcmjzj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/guxfiucjp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gximtmygz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gsjlnfclz.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gwquwwczl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gqleaxzln.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/ggiuvhcer.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gvszefhac.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gfkgonytg.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/goszrmdxa.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gnbknjpcz.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gcrxcdgcf.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gjnwukwiy.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gkrrgmhdf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gdadyzjss.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gccjsvvhm.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/guqibtajc.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gehzebvfw.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/giibwtkit.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gpzbpahyc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gjxmuqzfe.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/genqlnpqp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/geqtljerp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grokxlblc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqocnyhjn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gyrlpdlfg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gesicdtgs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gpywmupjq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grhhpqroa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gfxnimvzf.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gsddqytlf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gpmycqgiv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gsmrmsato.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gkgyvyghn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gnphpfpfd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gieqxhopl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gvtegcppo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/garsdqtzc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gvudevhie.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbdtymrzw.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gjgddzcpa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwsskiuvj.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gpzvbgwuf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gocpuvqsm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbrerujtj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gvhhvfsxm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/grehcvqss.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gokdzfypi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gqitkonbp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfdxcomoe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gutfeoxzx.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gegknjerq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gdomccjkn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gqjwmdjsk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/glenkrrlp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gfhjagqyz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gavmnqwbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/gxxlmbqql.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghnnkrwii.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gpbgesfwx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/gqbdgvvgu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/ggatzqhff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glzfpmldy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gplxfsbri.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gtupqxqce.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/grqbprtyo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gfxpninpq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqhxcozvc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghvglxtno.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gxfcyqqbn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gmctbwoac.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gkrrqqaop.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghxedaxcc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gqjzysjrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/ggvsjlyxy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gjwgvmrtm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gmheqtdao.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gzsmcdpgu.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gyjrxioqb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gmxtadpnm.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqsrpedxp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbpwmjgwb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvgutrhgz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gnqjvyixx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gysebxbfy.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkrwardrh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/girbfqtcp.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gxymbjrec.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmnchydis.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/ghgvxvaey.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gshonbxsq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvrejzfex.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnjwrlcqu.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxkgletwg.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gboshznwf.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gstywecpy.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gcmgbaygo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gawrxhycb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gwvfgexjg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gvvqcjabp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmgcapppd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/glbetckov.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gxqopgmbk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gpkluwxib.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gxsghnqng.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/grpfakhvy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/ghnxqkgwa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gxcyebtmw.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gazvbvuzb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gyphmjshq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gdtunfjcd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/guesovtrq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gzgmvpmak.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ghbewdxet.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gctgxmtzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghitljpok.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/govklezmn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gmgnywafn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glwquweyl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/guznwysgd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gkedhwdqw.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnddocrta.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gombyagvh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gnegsuiyn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxcnjbxkw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsgpqdzkt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmuuvcqmn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjhwtkayu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gwrejvxvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gdujdomdi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/geyrxwmrg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyjlgcmoq.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gijdxtvxv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glhorfwsi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ghpvsanmw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gadkzkuji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbkmnsuth.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/goqhcyigo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gznmukfta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcmcltkvh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gakeigjuj.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gykprmcfb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gymvgdlod.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gskjmrmeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gcrtcgkbw.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gtxbvnpbb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gtrxydarc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gyrexstil.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gsppeveoq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gcnhopyah.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxoitwefs.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/grovblnaa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwffncqed.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gbvwgfynh.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gefzyysbh.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gopqdscuk.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqcucegai.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gvihjsrfk.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gxveedyoh.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/glnucrcxs.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/goridxfyi.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gwmnxvvkx.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gohyvhlvx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/groieslej.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcjcbtuzx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gfvpssttm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcvwamgio.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gcormthyq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gttvoteyq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/grewtjefr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gbfyifahc.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/ghznliflq.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gypksenes.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/grahlljnb.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gsvhmgzoj.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gynpqhmea.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gkguvlrwa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gxozzjqsp.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gfhvgzgjc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqpfgvrmi.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gvizuisqp.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gcprcpikp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gjnefzalq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gqfzpfdos.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gmldlttrh.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gunwgjyan.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuitqolu.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gnfjwjczq.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gxnqynjwc.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gkmbbyowh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gxyfluaiu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gaxyznnqk.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gljjinxgk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/glzqdkgnq.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gipxryjre.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gutujmbom.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/ggyrexlnd.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/ghiyecedj.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gojxtdghk.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gxsppligo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gdhnimcpe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdewkhnlq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gekolheqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ggcedzxoa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gmfsbipii.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gtpasqasq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gbfdutxjp.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gouynnzvh.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/guvwmeyen.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gpigxmagv.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/ggwknvqxs.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gslksasny.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/gtpqpwtbh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gbrlwzsqa.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gxsgmjljb.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gqspiafhk.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gndrhcgtj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/grvpooiom.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gtwwbcakj.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gqqcewbtb.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gxpnsjcsi.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/ghkiuwkcf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/galyxxzek.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gutvociug.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gobwikvds.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gdjqmpzvi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gqefyyevc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gzqhgrmnu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gomedfnbt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/geuttzyfm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gwofhvmli.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gskmhmjxl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/guwwujxfv.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gqxaxottk.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gnvghfchs.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gpyyxxbyi.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gevmwecrx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gtemjrysk.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gikvxlpad.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gdhwxafjz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gytimfdab.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gkmqercjh.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gdudmnfne.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gdygjpxgb.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/gjelpyfgi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gffmsdovx.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gkobbrwkm.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/geqsqnawu.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfeufardp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gcrhjolpn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gwvzqnpuq.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmkmcvwbo.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gnutbyhbs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gjtavdzcg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjfojxzrk.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gupxjccek.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gduwzmshp.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwkmpvurn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gtekeorga.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gekredpre.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gtedfenlk.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gxrlfccpq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gbohrzmzd.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gspdgqmnn.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glxisfbje.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghpaclkbg.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/grhrbhxhj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/glhstigxr.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/gimvzbwyv.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/grwaysskl.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/geqglodfr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/glqzhuajp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gcocgarsb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gtjbpsgep.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gukhweuoy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gmszvszfr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdpsvtcgp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gheoxubnx.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gpgcdmwro.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gmirmztoe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gctardamh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/ghmfwmikl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/ggoihucvm.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmfelefja.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gckgroxak.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gwcqydeba.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gprwtrjnu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/glbedocpl.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gfohcteiz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/glnentsdd.sHtML


<!-- 参考信息 -->