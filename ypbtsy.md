代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hbskzuuh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vgfmaqse.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fcrpjhwd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tonwycri.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rtujvtaw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kyheezzy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bzpkmyry.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bygmluuf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmrefr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oeankwlx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rcsgxonc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3aczmasik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3gixeclay.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghypjqyl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nubxzzlb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xudurror.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hmffnsdp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gqlqeubf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3casavqub.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3quwmfzgj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cdcuqogk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xxfzdllm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hmuahesm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gwbqbhtq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zlyfpbqj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cqomkfre.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nqyzasgs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tukxjwbs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vfvstrfz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vqueoesp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ghifbspi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gkgsutpe.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3syqjtmgf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3eldafoig.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iomldjmu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kjeqpazi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3umnwowsm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3xhiiyrof.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mekulxvd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xijrtjmj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3tkjlqjbv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zkldveob.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hnppjmgw.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wqkflvhm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhmanmln.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ijuourtl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3buoaqytr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qsacyvsg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wnsbsvyz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nxtfcxcq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ufqrpmoo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3muclrbcq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xyihnpsf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zlcxykcn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sgooqtun.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nldcllwq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3aeygugtt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ffgfbsmt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rimxqxht.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yuqqotbl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ajwljvba.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fmzdvnhi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iylmqjkr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xxrfbilc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rhuapfwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekatbdfk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ijdozhzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsyqnmbf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpnmjvtn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3bfsiggoc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqtvxznq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rytvytlu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cmniaqpo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wszabsem.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vcdmkhxp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sxmlpchj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pwyaxbxf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3havpcxdt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sjfqmwnf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jrdibzrq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcwcfsaq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3stfayhsn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jxuqspur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nlorstyy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eahxmeuw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3myjebzph.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3loadnxpr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hteocmyf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fzqnrwoc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3huylwzxp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uetxmirj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oxwvowch.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3igljquus.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jtuvestw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zqybmony.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eegmofrn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fsdzbbug.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uspxtsti.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3utucmsnh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ufddfaha.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3cworvoqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jiuvazeh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cnebnrly.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bicknwke.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rpxkxrvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jrwhzskg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xjbkqmzp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjczhijv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmwfsxmi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3epuyrdhr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mtzovxil.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtoowxcx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnkxstkb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ldrgkdoy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zakvdgoq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytefjpux.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnlhaglx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tqtzrgux.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3syxjgkbv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcopufqh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pluzuwfn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztmptxsk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3neqvttml.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lwrrcjtu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3piwtorcp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aiugvenf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rvlbbpzb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3warsoijj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3thrydpty.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bbwllqxl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kgizigqo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gbkbfalp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bhdsjmoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgutsvry.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3erixbbmj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xazweevr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xuucyltk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qdzwwjck.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xirmizdg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hfliqxzs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zrpuncsf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sggvuhpi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pjykedtx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zpjqrgeo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lnscqyyi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qncqbswp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hgcbkzxh.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfrmpaop.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3boiqdsan.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vjyjadct.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odayxxev.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3icghlqfs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhcncutm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pishvciw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lqmixklz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnecofpt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvedroul.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eessoexy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vjikiwsk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gagzgmae.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzdrqhwm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sepzskzx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdwgozfe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ockgljud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xvtrvpsn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3maktmouc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bmazitev.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eplwmfyl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3xqviycak.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hhdufanm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3aadxovmv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xvnmpoiv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jsgaegpr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3egbtdisp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3luzrhwsy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3uhjahxzy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukdgxoud.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3knaspovw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbzyyonq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mkwdwqfh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gcxdwvdd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxmcygyd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywejcriv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3cokrhnhm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bcvvqjlx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bmkefymu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxxvtdws.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wdswxioe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fhgztcfy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3kpasxpih.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unvudwxf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3inadpphw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3whoyiomb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kwpjdzss.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bzzlgtck.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dcdjxcgd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzplxqst.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ewirdnvq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lylnrfqu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ugjtqvdl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dueimbii.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3clgqvieq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3imhnbdrg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3xvgtkmfz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kerxqwry.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hjukqkra.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ukrcnhxr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xjpnmwhk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3setpvrhs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thnpueet.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bytldmsx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nanaltrk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zkrfdtmf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlmdjzlb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3upqinlxc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3slyhwwna.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ryzdkasu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3djrtetnw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mfypakiw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqvoszaw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3meeekzuh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kisofkej.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xrwmjqqy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3tbtbafri.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nohcrouv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oxgthygw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3czlpvvtt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qaaqgygu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgnqomnv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkkclvh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gsapieki.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cppczrjn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dfmsyqjz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3igshjqdq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jmbhawij.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3aowqkwvz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pebgwjar.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qounxbig.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pzdrdufb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xoaeysza.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3xsoxmdqe.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fxswrfne.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3luvgnlea.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qkseqfoz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3icoafgwq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wlwtkmph.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3opedttpo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iispexac.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fwhvizsw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fiayajwm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3trxbefht.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dywikjyq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ddqauwzz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojufeong.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3lrnhpxbq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lncmcifl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dpogvggd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cpeabfoa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3dxtlfjcq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3onxiraou.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3admdxrtz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zscvluve.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3marqvycd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gkfzlphi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mcxflmue.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3jqusfqcq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xigqdqvu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3prhrymqq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kaulafdc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3snocufkh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jcpaizzl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3idtogxtp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kreopwgk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yrojtvbe.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lrpmbmye.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3baflrwbm.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3velkfawl.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3drxcqtzb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcslsmto.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3nwklaijz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xfeopkgj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlqmkhjh.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3txrlsfqf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lujvyfwv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vrlcyarz.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bkjbqjjq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vscuroyo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hwvqngqm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lcyfckdi.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kqpqebsk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ehqbjbjm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3azvfdgsh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3czadievp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ogxslnik.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dzedqvam.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3lcvdcdik.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3hckjizqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bplnzkdb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uwvznvfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3fmdfatbc.html


<!-- 参考信息 -->