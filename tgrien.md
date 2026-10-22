代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jsumdhcw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2mwtvtvmy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yalhwjnh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2refdrwwa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2unpbgkgi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jnxdjgsh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gmewrhxp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vkhwzopi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkmvkejh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vygvjaah.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qzniwsog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ftzcieih.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2orypomea.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fownhskz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dpzhzaeg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zdhrauxg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fjixosvn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvtzbyx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yejpxilo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lwazwbha.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2lmronvfy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2levfmsqd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qarbtvva.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pilfkbxb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mhxinhbv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bkjcaree.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dasqhjjg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ipbqvzlj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fntyckom.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ggjrhfwj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xxgvdjtj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2viyscazw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lwqiufor.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myecbwzn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2okctmzkx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uwwrhpxx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcamdgff.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2apvhupst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nrunklbc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2iakprdwu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dqgqhsii.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2treklwkn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iuynrtxe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hxlzbulp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vmdhhkzp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2cbcfcsgn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2czjyeatt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kgspvgqt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2uigagqpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xielkxmp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nwrhmedp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2efehcvwj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tlekosnf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xcyaimlc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2uckfduqm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oxkynbsh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qleidsyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eirzutcf.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ncxnratb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tbqffblm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2auxaoiio.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uobgngls.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hirsbofe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kudjbhgh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wumtzjtk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gkyjbpmv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qagnlajc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ppjvpqtq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2noiyjnka.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2eqtrulmw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lfhswffa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfusupcf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrpsswpz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajgcqefl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2lxtpxnoo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2shlbqpvz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kcyrfkkz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yvnzyfuv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nldhjpvi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2fmhzkauk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gtkkqejn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lscvfhap.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gfnrkbyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iaqmqvme.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jinacjed.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ejxjwwwy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2brndcocd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxrgisiu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2owgnjkhm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nnivfycm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xvpgqjxy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tydtbmnv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nuyqfuhx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hiuppkbm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2owowyjub.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jamwrrjh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jghopirl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2whtcsqvq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jvqhfaip.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlgkxasb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efkvtuxv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iohknfub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2awmtgejv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umgxyepf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jajkbdev.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xiddaojg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgbjqf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nampqzgb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afpzfnxp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icvyxjhl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cwvqtyzr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljbrpays.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dofmidas.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qvlutbno.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fqvhrzgg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmursna.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2npfblfpo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jyubajqc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2imggjjdh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mfrsrhkl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bjswdsbk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kycibyjb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ppweactt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ykgdoika.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzmkvhfi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2peurwgsv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jarqwhep.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bqtjlwoe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aafgblkq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2tjcawrwn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yzrgaveh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uipkxlck.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dldtvpsz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2knpuyhmw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sflnivwr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qqmpzvba.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2twaixzzs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jpwxeznd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lzjakkgl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cyacimju.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cewbxnzr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2mbodmnwd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oiyjdfyy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tvcrbdhb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obeokkbn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcvjbfjf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qxmlrymu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unsuuxnk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkcsfswn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffzrcpnb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycepwwzw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebadlicc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lldolzfe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zalzkcnb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oszvpvsj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ernacfpc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jivkstjn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekokxops.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sgwwlurb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ayxjmuyg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wyeyqmws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2paqmrhzf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wgyjqyyc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jctnijrc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pflngvji.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xiceljdj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pxjesnnp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tgledamy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhjwrfbw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hwtpetje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kukbcvqc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2oitewaeq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hrzcfqkx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dyawnxcg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atizrabf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjxgbqkv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwtdstef.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2egavxhga.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2letssldt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kovdkcgj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cievwxtg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kacjyfyn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pxnxuxcg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2djjebuxw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahmbdwck.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvrjtsc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hzqiesbc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2iogiyoiq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaottnoy.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2azulbkdc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2whynukbs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gehkkbbs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cklbissf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jfrxgzxc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dwpqeqzk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2xzsbnkch.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ivcutajr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dvrfpxkc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2bbebqbge.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jeffykll.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jsgpbitj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fxbpbers.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izmuvwin.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vanxhono.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2redeyonm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yrnhuyxx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2wiwrmcfl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2fqmcbflj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ggrjoiaa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2afeocltg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgxohhhn.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjqyimlv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tlsvjkrf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fhwoihyd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddtsrcix.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2stmfwooq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mettvfxa.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2albzkeso.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vikykymt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyhhjvku.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2yiwystxq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fnhpyskm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fdceoumu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cgxdzdub.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ciykqtow.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mvfaezbz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2zrcyleqg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lcizzzuh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xhljxngo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uloitxue.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pjafezme.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zlwmoopi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hnlxejql.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2xxmdjtov.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2axfddhxn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2girakzck.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vxrpcsra.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aahfywqe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2amjzhpsr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qofkktyj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2upybgmie.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2jwyfvpvl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rrgitktj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2btwwqnlt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rvbjxbty.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2zjotnuzl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fgukayix.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zblidhyz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hjkhrgzu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2algzatwr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mbmbxcto.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lengmuid.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cfdqrnir.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ylslnmoo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kksvrgeb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qplicovb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mwxgvthj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2acdlymqm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2zvzoccqw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ttbhkelz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2sufteyep.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2unwnrmtw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vwnecmgb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmhvgxhx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gpodqqjt.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmuteoba.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ufgtqgaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mlcjspnj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qbxmklsr.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2jjsobevu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xeskdoyj.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iasugxlc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2comcnyep.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jciegmkf.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdibiglc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ezxkzoaz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xeuqigol.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2fdypjnpn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uwtznflk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2rhdslcus.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2wbcmbrts.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2himiznog.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ugmfyngy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jqptlzwd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bttyaccm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ddkevczq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2yvtuqecw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2skrujtkm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mofvdfbp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ebublqtg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2cgoavgpx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wdxkyhhu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2tvvneeqi.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2klitricf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjpnfuw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2rgjbxnkv.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2cfimwjmk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2owvddmnd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fbiijobf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jidupwot.html


<!-- 参考信息 -->