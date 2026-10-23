代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dqorlkcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3whaqzvdw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fuiitwmv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vnnyzyki.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdwwjmkl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ejxdasqz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3keykwwfa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xnhcgbfi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tblyknxw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dizaqbjd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3vpqpgvzp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpdeflp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3exkxjovg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hhjwidyv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3exkhwysy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eskadfdw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qdduowrd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wpxprlkp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xhxwswtf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zamjzgbt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ocpggewv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3luuyxbym.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pggevxck.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kyynylcp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3urvhhiay.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hkpwsaqo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qccglhpz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ahnprbpm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mghmodqf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xqzypxce.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvvdwsve.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3njbqqoby.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjnmekcx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fsaiyref.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbeihahi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fozxndni.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jomhbmup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ztaaaxrm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jbqxztsw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jcmsvmns.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yskksnbk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kmuwcdje.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zdqiwxou.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lswwikmm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pkbfwfrb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3elsbzdnz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ikjbesve.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xwzkgxgz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ilpjpflh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ehzqsdpq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lkduwfeg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pdjjbcrn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yqsoptvf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkyrxzob.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3sknfkvqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijegkxrk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zabyopeu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lnojpygp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uqmgwdts.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bpjgdbux.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3izxfhqze.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xewoenpb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3chgjlpft.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzviwksp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vgspwmxv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3crttnwcn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qifwxqzu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwutciyd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3geyzlkvk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3drgifgbs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3lauynpms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bpwnzhps.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wtcdxlem.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpzdlov.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3tnwlzxxs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sqtnriro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xnybatoy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mponwdsm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ktfzzelr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3puomkxcd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ogtyhedt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmrvgga.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3okqjfkcv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3owbzyjty.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uubpycsh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wzkhvzij.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3coyprnfk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqcmmjix.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vmcjhqzt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hkapgcom.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zjxvixir.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3efkxklec.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3whgvplxt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iowaprqj.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nbanatnb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksqnpuaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hiytekto.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vlxjawrg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rnkhlkjl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zttrqtwv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkpfrzrk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ucqqcqlv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfrxdgrn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lxudcoym.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvddzdix.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxhbirju.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3skfrpkkh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skviqmww.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbdfujnc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tuhnjufm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3iyothdmf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3yjpaeghs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zkpknbzn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wzyttssb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tyfndmbx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lxgjskle.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3tatpiykf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uxgndqif.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3crdwgbbb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vpgwsdue.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tdvfzdtl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlcytdpg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kfaxbefe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pawsqbym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3naifhttb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fgmxvzpt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3qoxhcemg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vgcicqsc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3pkajokoq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dsnmemso.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ttwmliyy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lpckohpm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hjntkcuz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3njrmcfad.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3adqnygvd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eivmqdsq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3awkvxogz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rucgnnpj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjubjgnt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqgkkhnu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbegejjn.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezoxgdrq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3djxfpsev.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwahewyg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrqwcflk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgujsqvt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3swklmgqs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwgrjkzc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ptkfyqwi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hoqwlpbl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rqpwyrjf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3drnibdhi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pwzzefeg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uodaidnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vdtizknd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vttfbsgo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yifecpit.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tjiuyinn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hpzwrbzc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zoljylkv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3whlrltvg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3irxpcmfq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3dxqoyhps.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ujtijuni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pvahvrop.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ccrrqbpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yyzuhjbv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3deckuhil.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ttksxvic.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmszclji.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3idanasib.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3amhphkhp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wsfoudyy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gexjfpyf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3isawgrxx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmhdujwj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3dzjdwgkz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3uptyauex.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gvusvhxl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jeyotuzy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rddrotpx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ytjgrbul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zqdbmhrh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ifecbmhe.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mpwgsrgr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ofqgnrcy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sgwtcvfv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qerqktph.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xaioywgv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mysmwleh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uneaeryc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ljxwvhja.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rgstdazd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vzesqlfi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ztiknrfj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3favdcopn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbcowzci.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lknuotev.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kkzqniaz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psexibiu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ngjmtlaa.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ixhmfebq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jdzslrhi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3aaqlphkz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fjevhvbq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3reheyyhr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rdspbqcd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mgdwrduq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yecjmxja.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qqebszza.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fbftmwiu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3apzgtcvr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zzclywax.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3csvshdbj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykqmmgto.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wibiylrh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjydllss.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ukuwlcnm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uwbqvutl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjnqyqpz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uqclmygb.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jcuuvthw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wgapqjgc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3drybvmst.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3igeiernu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uobeeddj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dwvkyjkq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wbxxqjlu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wberhltf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3rwjwxobs.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3idjgiigx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qkgwhtaj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xllhjwjw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtrcipun.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybgwflls.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3mpxrwoud.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3skpiuhkd.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lprhqdor.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnhjjegk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3mxgiaiql.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sxpyxoja.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3xennlert.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3yxpyjhct.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uljhczsi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3snwpxftk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3urdzwqos.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3wxrtcvky.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3smcjalad.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3toqatljn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lbpofcoa.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kpjdumqo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3lekxszkr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kvadbmnb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3lcklgcou.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3aoppejks.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ukyduyhm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ebcybeuv.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bhnjuitj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cdllysjt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wybicrel.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxvvxjkp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yigqhwvh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pokmgmas.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zqziyize.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ixytkyku.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfavfsjf.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ktwegksf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wqndnuit.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jjfiqhoy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsqfnqxr.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsjyfhtf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndjthudr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmjlyvk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3smshknwq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ibfuykkq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3tcayyako.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3npahksdr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3msglonld.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yujiieqs.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hxcfkusk.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3aikxlype.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3tahjydvz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3uzvfyjhj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fdxufxqx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wmjyssju.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3jsxpquov.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3churflyf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3moyywasb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3cwiezoib.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvihveyq.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3pgkoqtwg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3bxhswonb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3csvbjsem.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ubjnrcie.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3dwtcvxow.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3wmydhfno.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hqfwbqaw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3dhmbdxlq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ftubpuse.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3dxlvabeg.html


<!-- 参考信息 -->