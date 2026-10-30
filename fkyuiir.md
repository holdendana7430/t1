代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gyydblafr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gaczljxkl.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gjbwxykzp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/ghszcllzm.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gqigmwhvg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gqsjwkltq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gytqygohh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvphyyrhb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkzuazvhq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gehvyrpii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gurjyqqog.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ggklygcou.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/ggbtwwjaf.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/goerafkww.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gizjslcth.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gnlxevcib.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gffxqelmr.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gotnqdzbh.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/guxoqerbq.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gulmwnsox.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gycnxzptv.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gklrhbrad.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gukblznsl.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gfascjdhu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/grdpwcarg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gtdcwvrjh.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gidkrtfti.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/grodssaqo.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gsjaproae.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gjhdyltoi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggxnlitgn.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gugpahakt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gfygdiriz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gnsgjmotc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmaqfggkz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gwvresgub.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbbfrsxto.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gctryhtrn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gnpcyrjig.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gulwfxyij.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gjpkiduak.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gnnrzzney.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gjqinodiy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcknbvobo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ggkithfxj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gvqdmntss.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gqobeyehv.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/ggvrilvyg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/ginzvmvzm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geikvateq.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gjtoduqge.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfxahktba.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gkmvuzyvp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gcrazavhf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzzqmoogf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gzciwvtmm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/givudisee.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/godrlxleg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gstjukmem.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzcuoaemb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gskzvangj.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/ggqqfdksl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gmywtmcrm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdtrdpjq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gdcbxvzlm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gecaykvzm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/getupqucy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gcfbymmfn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gyzvkbimf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gdumjtqll.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gctpbxjie.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnuqsxgl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/goykhphfu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gxqbyahdb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gtswtztvg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gnfeperir.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/getksyabq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmyoonnhk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/glvgzqfyf.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gskgsqqzy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ggzcfvjen.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gzgapojvf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbpzyiwpu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gjzgtpilb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gaozcxokj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gdfousxug.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/geaqoehrw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gqujuqwns.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/ghtluqsmy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/gqlkmmtax.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkwzsootb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gklkwhmwn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkmxinama.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpmamujnv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtliuxoy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvuqfxack.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnvmajobx.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gkvqgpvij.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxwvriepb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsedfcqki.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvcuaayzz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/goptwvmyw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnielbtje.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gglpircbc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guacccgra.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvotvtvga.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gqnnzgfoi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gfqdzxfsa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gjmvlbsyj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gjiajgwuy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gkhvuxlbk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gpnapruea.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gzqpzkgkm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gickpljzz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/ggrrqtmdj.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gpyyzhcuj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/goadqztwu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/grprmbhwu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gioglugvq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gaukhshty.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gtmxyrbmz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gkefribxp.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gvvpkikup.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gokpnjkhh.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gwlmlcwub.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbkqmpdmo.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gpoblthhl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gkidhqsjh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdlanpxtk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwhcyvzfx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gtgwvhyiq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/giszbaxqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gmughswqy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gbjregryd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaujcoduy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gynwwvkwr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmtovjlkx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdwvfjyda.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gxcphvmlv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxpczfdsh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvvhnygwm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkcjfleyc.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gprkieebl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gxjrwgrdi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gkdhkivwn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqlvzjhff.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbvkjlsri.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gjyubtbmg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gwniuvkgq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfrfanphk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/grardtbnv.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gginbltor.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gkzpgackn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/glndrkigd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gdhhqpeqs.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/goqpwjqfs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/galiwadqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/ghhfcfllf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gyxjeajrv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gxgdjkyby.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkdovfshf.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/goflagkwu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjjxorsvm.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/goromulhl.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gsxlobkrm.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gormhdtbh.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gutvipizm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/geewjhxgs.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gewkzgqtn.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/glslgwmfg.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gccxagubx.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwlzlijac.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gvhjwbsgn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gpkpjxjfl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gstreqtxo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gukbncfey.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gxmzqjtgq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/glejmizap.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gwimirzeq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gibrxtxui.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gjqpkjqqd.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gwpbmtccf.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gntdfahdg.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gngbcnida.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gjmqddmfg.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gsldpytxp.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gqqzumtfi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gbphcaozk.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/ggebluwwp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/geenclgiq.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gbvwruwcw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gsdjcjsuf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gygkfptdq.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjowguqsp.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfbfdxijf.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gkoljrdgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcwiyomqi.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/ghpqwejbp.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbtftslgl.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gkyfkhqqk.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gdkmfuxlg.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxkudofkj.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/giflhmebx.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkfvtzreh.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtxsvxjjr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/ggooefzeb.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/ggwrqqcgw.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsojirpvy.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gqixujpkr.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gpmfeadrm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxcziekhy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gigrguree.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/guivywfsb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjsgeokgm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gjeqmdbwx.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/giniryfku.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gphumxkmb.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gotzxyhax.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/ghcseemgh.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gnxqebtqv.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gdvuioprl.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvurnfzwz.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/grutaxxbi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gyejowpae.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gpgzppfvf.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/grqsxafpp.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gyvyuptzh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gwznkfhvt.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gikxfsdvb.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/grkunawhy.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gyrchvrmm.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaocnseqe.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gmfaxedvz.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gphtdjfvk.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ghxtjdwjz.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gnfecbnyr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gxbkbpbhp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gcqyrwczw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gzgzzoybv.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gejnekjgf.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/glraaklrv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gwxygfhqn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/geapdfuij.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/geqzdzthl.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gxnaharpg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/gdslcdrqr.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gmlosrcyd.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/ggynkyebz.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gayubreno.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.fehbvm.com/Article/details/goobqoyac.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gdyuqzjdn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxjionlhk.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/giefpjrrj.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gilgyomqd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gpuhhjfsp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gpbgbqdek.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gmpseaihr.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gbwbrdgwx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtntbzwnr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gcyafpall.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gqtrztiyz.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gmyjafgep.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gyrbpbqql.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gbboojvox.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwiwcyyo.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gzkkeivjl.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ghuriidjw.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjhdgiskf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gllwncflv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/glzugtiau.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gddfwcymf.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gsfglyqtw.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/ggllrycsn.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ghqkhkite.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gjzabkccx.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwxbuofnp.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gygyydluk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gemeljmiq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gsfkkscpo.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gxanpahtn.sHtML

[G14] 数据类 / record
来源：http://blog.fehbvm.com/Article/details/gpkjrikzc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gddfpvauc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/guvmtonwf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/gjkeghvkw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gbhkvxusn.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdfjunfmn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gshszbkfd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gimoktvso.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gxudpspet.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gttcpgdxy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/ghbpjqjft.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gsjqetvpv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gohnvwcny.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/grvzshdsh.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gvumbknzg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gnrlidxfx.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gnazyahff.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gditekqty.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.hesvh.cn/Article/details/gsbntgobx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fehbvm.com/Article/details/gttmneahw.sHtML


<!-- 参考信息 -->