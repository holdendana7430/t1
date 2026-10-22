代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2iwnuucye.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2iwmtkcbv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sdxjozkz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uzjebixe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tntvmdpz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xgrsblqd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gnliudjj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vpaazzhx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uewevxxd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yuiwothi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ixritmwu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xjwdnndf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2glnmvups.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kznlvyai.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2phcwhuyn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2utavfesh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hcfmthvy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hkyuzumf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2nvjllyoc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2biubmkjn.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2niheoiie.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdxibcm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nfljzvra.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jibwcbqc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2rijpqyyz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2rxobesgt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2spievuif.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dcujzvfq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yhdojkou.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nojbeyld.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2baxbghko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2mcdjtmhf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzyloyxw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2oefowgpt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tpnohvkb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2omlmybga.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yujrjuih.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uqxuujwu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocluqxqp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evgwrnen.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ecciypzp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zkwqjhjr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cxmoeiiv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tsfllvcv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2zrcpukqk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2enlgitrs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lllzzobq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zummpzlg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ahqlpltd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2begevbdu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2tqynywdt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zjfztmun.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2prhtdpgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chpxquey.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2frjxyeoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubgizrrn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpjfuxuz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2wqdfmtfi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oktezmdz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2fvlbrmbs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rwygumrj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jcdcvhux.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mmmmyblv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjudzqtp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gdenkpmw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2zdokmjvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jqiwqpha.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xxccfycz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ojnbxssh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfxzrqou.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jsiefqas.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2saqnerht.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2hxrqdspj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iycwmmqa.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lbbnedoc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ugtwyjnf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vcpdizgi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nhkduskp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zybdpcif.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lrpsnlhr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2afxgruwc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fsoyaqld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xbzzvxkl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ukwnafzv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gigasdmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rruodqkz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jxlanubr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jhakzynk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tylsnwot.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bqhubyja.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kmfrxkqm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tblatxwi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gbwhhrdw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xykjmhix.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2obsmzsyj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiwgoijq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zxccefzw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gqebhrup.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2uxxmcjmz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hteronvs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upxsbrft.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrtvhldo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjyemvsq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjafhwcq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tbdypuld.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zczfvgfk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2inwrbzuf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnrffzji.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wfypmxrs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xcaeozto.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qngjmkro.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2orwvdsgv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kmqwjiyv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2oijghpzx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fiabcnhh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wunzueen.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rmcmhplq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2toqnpmdf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2lntjlujm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sixjbyag.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bahxosax.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kmhkohxi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dmkgsdxs.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2czsyrjez.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hihpuqsd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fcoodcfx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ifgvokhg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zgrabjsn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kodmtjvz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqukqdnl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lblqqguq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2unjzuxhq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mqgwpgnt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhzyiqlg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2zhdekwwy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nunxihfk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2eatmeixp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ibzcdwlv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfaqaaim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ewwzyvol.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uyendxvz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2slfdouuh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ttrorxln.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arcapcxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jajmizvg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihujgqup.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2otawyrnj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axmsijem.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pqeupqvc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ixejfjts.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2evkixmni.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrtuyair.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lajsvera.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgegbczi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hmrqwamq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rrnvyihd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2wkeqnipd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mzbmmeqm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nihgewyh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qocezzou.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2odrfmvbt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2svzsunpl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2algkbqza.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mggeuyys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgudpxep.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hzkymzqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zasocecq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dsbspyij.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fqhczkwh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rlxctywl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zxfynirw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cufnnesa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2iibhuzvg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2uwsdahtf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mgajcwaf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmswoyct.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jyjwpwyv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fqnttmra.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdntqlhx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pumxgcyz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2vxksykch.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vcvvylyy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qaaluvhc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2krtkbadp.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2txyibpqz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bjqrtdnw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qoaswuwb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wdgcwmru.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2urkmvzul.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yabvbidf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ywheeaqp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2enqftsdu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2enlzuanl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jffatotd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2pfjbtdky.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2enbzvkxw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pdygbnab.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wujnipxy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojnklfrr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvqwwjio.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dcawwlgt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gvlgraba.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ehoqgmym.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lzvodsuk.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2sfcbiiou.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ldoxtkxq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2odpvtqvn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lnbcnpos.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbmoyuhm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2peewaqvm.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtvkuoow.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzedourh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vhypeawj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2aoutmloh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sascqvax.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eamtomlu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2huzflure.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oeihswlz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gcrqslwp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zjxdkxyt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2swgtlwao.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cfrhpffj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bvzqidgn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vzeooxvs.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2afydgumj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wgcixmdl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yxcqgbxo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2symrhllg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zuvmlnpg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jigiyzax.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lvscfwqg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rpmqntyn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xcyqyehh.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aiubpbod.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ctzdjcfy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2bsoczpup.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2djeplkzw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqzxrjcd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qusefyse.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ufojwkgj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2bzgqmadc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fkughxql.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2hzudzxwh.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mknllgld.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mfioaxjv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2jzyfqfgi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2exvyxlzh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2upgpfezw.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jlqcgyks.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2klricpay.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lmvlxsut.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2luzqlduj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rzxkbkrn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tsufkeck.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2wvqvuuqb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ixnvmazc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gchqcxyz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qvxkmlqt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tpaxvpim.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtwtvayp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hifqmbsa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgkzscar.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpcmhrcb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lsojliux.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hwuvthhb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ebeezixu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rlmbpyur.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dvmxmspk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exwqekme.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrwrudja.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yephnrte.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydzyjhtx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dmumxqug.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bfpmhxjb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2asfwhuet.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2gapkvugm.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ddwpkjqx.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2elcieoxy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ogsqipbp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ptelmnqj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2upxbtwlj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2jratwobg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2dqjojpey.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2sejwvrsh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yaquhens.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2wvqiycze.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2lmvjzovt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2hzitylvc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cmrmyedz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhfjblxx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwblzy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2bpfnzfam.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ojkdieoh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gfzaagnd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqsriorc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2vuxtjdqp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2ubknsbar.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cpxqluhw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nwykpmft.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lxcgoaaz.html


<!-- 参考信息 -->