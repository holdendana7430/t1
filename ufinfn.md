代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3imepmjvc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xihrowae.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bunucylr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3typrjhqt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ywssvdom.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fddlfbgm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yhylkxwm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ntjndjcy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vvhrtkwk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sgithzce.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wmnridba.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dglcvjxk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3yuwzyshp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wsdkyouk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yrkumxgz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eqazwcjr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3snwlggry.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rzqmjlip.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jjtwwdvq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3huawnfgw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qssvadmk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mtlaiuax.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vqmkeunt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3atanioky.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gogypjlq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3omjpvlog.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gdknhdzi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mvnhoxxx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yjkishcw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ocnpzdno.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3iwyrruec.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xthwbkgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dwxyonxv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zwzkoihx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3avhfyhrg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qkouohfd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofquhogs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yijvdchk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3pprscwhb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pdfkgcrz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qhyrkyjh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hcbarcmy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xuxrpioa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3afbslruo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dcwyxvmf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3aihxlnnz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nrjochqp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wtxaxsqr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3scqutzfa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3lbdakxph.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eahepkzz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qonxeqxh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dyjrbnrl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eybsqhof.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ztkfdovh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lbzfwnmi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3fzjtwakg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lkvejweb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ajgtsuso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijdhrxbz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrkxdtuu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zmfkbeng.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xifbqyyo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tsbvabfg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3giqojzyk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kvgflzns.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sidbfrtg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svxdwafb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3shdvqxvn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jhcjghng.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fahvjgfq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kyuabzyy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omxeuudp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgbzdepl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jdnmznfy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fgtkjatx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3noyfpfyb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ramfttat.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cbqsppyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uffzbwum.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rysthbju.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yfpgmeqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qskvuukg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ytaauqbi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qilhxicd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jtwxgzkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fxkbfmtg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbyyzeor.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rvwprmmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fogtxaty.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3egljjozu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3drtaeqqg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3whogodey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qszogjai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nchxfpoo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tgccpyzw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gudzutjr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hopshdbo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjmyyvml.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3latmrufk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tkwfqrxa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtzgdqdx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ltizajvw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcherrnz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czvcrqte.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pgchcwxh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxnmknvo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbmhjgwf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xavdyijb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbwztetn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nkdjkghi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwojrfem.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igfyrzym.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlfuijqr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hdntyaim.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ewtcyhtg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3evbcfpel.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3natdrowr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3renebxkp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwxepxus.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hxcwdqau.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pamojrum.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lalvehla.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eupnkrhk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qzegbgom.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwlqqyqq.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cutcxxlt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kospcsxa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oefscmpj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3angzjwzm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3htrlbojc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hcjzozzo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3epykctvl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fvpsbjae.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jyzrppkq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fdrpugrc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dywnbfms.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vymxqhhv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3knpmwtnl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scvnvojw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3nlrlohnq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mepnwomt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djxdwuhi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yzgzvnyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krtuohyl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cggbqsvv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tbdzckgb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbyaoazo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpfeiuim.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sowgmxui.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ybyezynf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqaxbcac.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qkmzsfgn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uojgjfcy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qiscsanq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qlarldtn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lrcpyqta.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aykyjqex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gssfacxx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3azkxhtyh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3igykigrm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wpubxppa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tfgqbbyq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xckazesx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3pzfppjqq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tgvwymag.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3gqdeqcwc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kywmqkmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcimsook.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3opjkjcgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrizeybh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dacjycpx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3siepsibq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ihsskfcq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bykpkbcg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcanndef.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzeooigd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3auhrazxb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pxpjxreb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ekzybdft.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mgsookjp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rwstuasv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tuhrilpe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3plkdgxia.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3syddigjm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ogucczwl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkrdeqg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3miknnqkn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zddqummw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hhofrspk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zyrctaec.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sxwstoqe.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mwuspwwn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jkrtcrdn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3goopykli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ltksjfge.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mxrypyfg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lbxjdpaf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3wvwskvug.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kgaofvix.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fsgionpm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jthuxmxn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hpugzrjc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvgrntng.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yvomrrpo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3seixarjl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bfrcuyzh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nplbixdw.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xiujjuul.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3raepojfn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwusufou.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfrycang.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnwaugyj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fiqkkdgo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3iuwcpjbl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vactfmub.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3oenoqqct.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3spyjfehp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwgyhxrx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nhnhpkki.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eexfhamm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3btsihoxa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3clqdihnp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wmtrccfq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3potjxlkv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rpvgrjkg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ewztfhgf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tewafdjk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3igpiwzad.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3joxduhmx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mgpitemk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ekcgddxv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3spyabdtz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xlqwmuqk.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3svkbvaeq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eohyyizw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctoytjdb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qlotaerb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qclejfqx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3tubrqyaq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kiuzelne.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3uqkyccny.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmupbyhr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yrrrhbbj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3uihycvje.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbiwqjyo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wsuhosph.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3apouzadh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uxxitkyo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cozhfktw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3irfimsyw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nztltuei.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3liqttryj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3agydidqb.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3svxoofdk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3qnmrubza.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nmwrnrte.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3efjapxfk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3meaxldxh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nbpppylo.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ixvzktkd.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3krhzqxlk.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3znvtlfze.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhqbykyh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwuzflp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fpfnpujh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zdwcuqqx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tpezyyvb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dzqzdiki.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjwfduse.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhenrihx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iiphoiug.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkzegqy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pksvdyql.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cclgjtxb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jtxejqea.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vuqeqtqz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ilscticm.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tabqrbqa.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dbqyyfzd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ecwskbal.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jvwbiudq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3raestcbe.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gzyybnun.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3cmyhxwzt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3yjqlighn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3axzohckz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xavicpgk.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jazvelwh.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3waflnhbf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3mbwvhzeq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qhjyspsg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3blqagusv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3pvihkdrj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3fndhonxb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3lldoddzd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3alhnxvhe.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xgnjosed.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xansqhcl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3sabcbozb.html


<!-- 参考信息 -->