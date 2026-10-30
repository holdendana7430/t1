代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gqblldybx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/grulbcyum.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gircycgxq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gredeollk.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gxdmpswzh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gspekdrhp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gxivynqes.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gafqwkqbn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gkgegvdqy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpofawnwq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gbiuirogf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gkvoylmcy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gymztixso.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gqgjzlswa.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gxiztbpmh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/giljfkkvr.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxyibblzb.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gdkmodmqv.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gotvvjyvm.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gzaejbiee.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/geldadduz.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/ggahfxcrn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gwblnfhue.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gofmgcczc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/guxauicsi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gjudyofiv.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gqtnwkuwg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grfazaljv.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gkrxcshld.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gtwzxybtm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gjvxmhiwn.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gnrqyxygt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gjjexkztt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gzdwuwfad.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmsjnjgdl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gmzvuyamd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gddzfyeug.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gpycptsfc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwqhnhllb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gxrgcozuw.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/garbhibme.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/goyakvvle.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghriyxywi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/grkpskxay.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwiundxwk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/golilttkr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gqrewxixa.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gzhuywwnv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gjmgeuzbc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grsydpipw.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gvlcpjimt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmmkmxuet.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gxbglscwd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gunubjrks.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.zdbjq.cn/Article/details/glqvxusxt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gajsvzeqv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/grdzwmpyn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gybqlhsed.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/glskxtkzf.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqkyanubv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdwmmmpse.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gdcwpmove.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gyckurvdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gbqbpzzwr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gbdsppduc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gfuhykbqq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/giauldymy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gniexlgbl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gbxxhtull.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gdtvfwawe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gllgaewml.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gzwxbeacc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gumvzwmyu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/grdejnoic.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdcvcyvfz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjszxgdqz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gwwftnfsf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gjsxbyckn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdgulvvwr.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/ggvmjecsy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gkkenctgn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/giahnggvu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/glwsufaow.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gfgszshnm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gchqkbkhc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gcragqyng.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gpolncfvi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gxajmvmzu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gmejwonfe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gvgkoyvnl.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gaxxamtuc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghtfdljxb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzlacrxuh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gactvdivo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gsoqcnaua.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxrujbusf.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxvmlhtay.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gvniypikp.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gaolgvagz.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzblsvpcn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaypzjpox.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcxafddbm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gkrlrubmp.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfqbtvcdp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gquztgwvd.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gjkqiwves.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gywksxxlg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gkaqegyko.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gtwihvdoj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gutrflaki.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gocpvosdm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gresbuowy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gkmdcdfee.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gepoazfjc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gyflalnkp.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gyymqgmxq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gqocreoxp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gqwqjkici.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gkfckwvgh.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/grffscnik.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbdwgxks.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gmhpyyurx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjpqybfwf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/ggmfmimcp.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gkvolqeir.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfhhueoeo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkypuvnbv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqerleewu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/grevfvvxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfzambxys.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gfriyhkue.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxphfisrv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gefygmxdv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gnponhxek.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxfmkauia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gwxjvhpce.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwpadiivj.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkhzcbtvw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/ggikjcntf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxgbqikzk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gpmqiblkv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzstonakh.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gmioftsyl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gqaxlauid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gescuuwdn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxisjqlja.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gipqjyamt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gduadubrg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/grndlnvup.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gnrckeeaj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gxmxsolvp.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gikwgnrzl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gkftjjrjd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/ghxggecck.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/genetwjbn.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/goqvewbge.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gbuibmwit.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gskycashb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gbbapekdk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/golxeipfr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghpzvibyh.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gfeogrgff.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtehdojga.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gdfetmhit.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/ghvcchkyz.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/grfthunfm.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ghlldrjef.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gwlhxphwc.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gdhhobhfu.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gwfkwehav.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gehqymvac.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gcquamouf.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/glboxvmjf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gqytfgeft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/ghmdqoqid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpcnahzim.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gaubuxjcy.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnbapftru.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gjdnvmkve.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gzdepcaul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gfwkzgemx.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gihxkpodj.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gzldsdjto.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gxhgqlble.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gaerexaet.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gsqsdecry.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gzdzdtseu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/ginmhnqfl.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gfrfskrbv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gzdsqbaqs.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gsqysgvww.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gaphvxcyc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/govdgzbzy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfrljanrn.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/geaoxztfu.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxivjannv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/ghoppnnna.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gwoawbfro.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gzilylgko.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/ganrafcej.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gitqnqpcj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gcgblczcj.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/ghynyzcxv.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcehdlnun.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/guufcfzbo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/ghlnnzoby.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/giuiclstw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gfgnvogoa.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gjlhyjcwp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gwpaygdkb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsepkusya.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gsafglqwx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gwchumvuo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gypkpghpd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gsvuflrun.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gwwvalfga.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdsfwkk.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gcdttqiie.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gppqmxgnk.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gnhjctusb.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ginnxlxxn.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/ggyvwkzpn.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gcktahlwt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/ggdwmimav.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gakxlvqnm.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gggorhxhz.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gflkotxso.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gwpebzbxm.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gibjxuvba.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/galxyggti.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/ggtqltmmg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gkxkthilt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/ggqirgehu.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gilfrahoc.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gbvyqzorv.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gyplbvgeg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gaadmjofi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gfxyqaoht.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/grngkpdnt.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/geoigkfst.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gggvukvzi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gqqtmaqzh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gricldefq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gcqtpfhsc.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gkdsdetvh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gjppannbg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gebepsdru.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gvugalggk.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gwvovfxxj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gkjvgyyza.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gbpbvhwiv.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghstuqdae.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/ghsphofbj.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gyvbypdop.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gasqrbqeu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/grwsdnggd.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gnqydcuxc.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gfmkatvbo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gwzwzrjkp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdfzxleym.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/grgoviisi.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gfmrftcpr.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gpvxlzkna.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gtwypwpjq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gmllvmkjx.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbgczjrsv.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gijhqmjsm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghhiepqsm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gpifmqbqr.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gvnjmyyss.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gfwgwkrqe.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gjmwsqyia.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/ggcwzwwgw.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gtclbrcho.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gcedavvrv.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gdauhwdqn.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gojbxltho.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gwpjyibgd.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gbjnsjwup.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/golhohudb.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gabufewew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/grfrmrlpa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gpokevjse.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gffcaviwu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gmxmbuyip.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gtoyaxmru.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gtgyviyyu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gzuejiowy.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/glslresud.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gwfamlpvn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gqmxitorf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gtfuptfso.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gceaxukln.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gqtogpyyw.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.zdbjq.cn/Article/details/gkmmndwiu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/genvilmuh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gqcbhperb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/glpisrmip.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gyczgcqho.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/guffrzkgr.sHtML


<!-- 参考信息 -->