代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ttzikeov.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2bxgtafde.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xgzcpdle.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2odnajcei.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xtnyiasi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kdfzupdw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2llsrwwfx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wzdcbnyu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ptpxiijf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2sfkoufxl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hfpcqcwi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zcnflwnl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kugzarbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2opucjkwo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wfbdneyz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bueofjmo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ttsjgbyw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2tcnhzdvs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lrwhmwmv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tmtvpjif.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ntyvtjti.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xiirnlin.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rkcefvnz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vgcjxzna.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ckzgiobk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eolkhhyh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yjqjblth.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xiokkunu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xttbtnjx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xkvlicvp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2amjexwuv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2arxsxsni.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2goeeykua.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wplmutau.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2bjbvoohw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zybzmsxu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2msyffess.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lhmvylqn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2xsunmpto.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gsjgkcip.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2sjqeikjv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kfoauglf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lvbakcbd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tksqdaup.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iftasmfp.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2irxpjdpi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stqqzxmj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2pisudifj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cqulgrys.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ijajlmqv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tgxszbel.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yjdfohvf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cjyalemr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mjldmfbe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zcwlnbgn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ykmaztys.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2rjqpnskx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fgtvyizd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dzucrcyn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sypjrrkr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bhzwqann.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qjzzdvtl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fmampcmx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gyfvizoh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lsirgvcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sujrppjb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bhgdzzna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxvqaszc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gforvpbw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2amtnjfzz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ktzjhpui.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oksduvge.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wvcgteaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vhuiwqyt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2swhvkgyd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wepdzfel.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gtioakrr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mihuycez.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cqoowpfl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2dajtrlzx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngrvlbmr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xqxmaimf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sidyepds.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pcghibgk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vbfczrbt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdmtdyiz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zkvfycsr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aqutxznj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zphoxrmw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2znudtovg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zzntqsuf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zkphrlco.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2uujecvao.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fawzccyj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lkncaets.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lroubssj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sgzygxrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lfecpali.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vnaldhua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yivrkzko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ucbomgud.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lmprjlav.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wfojtler.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2imrnkywz.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2offtaxje.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ukbylyhd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pbteshnl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfnilwul.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zlhjinih.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dmhucwlu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2etgtbemg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebfcbypf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyvywccu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qocivjzq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riirdmgk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bvprkpqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqbyatny.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewikghvy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2znfohhdi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehutzfhm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohiybbwx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wjrjwbdj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2uzqbjlfm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2asczyzhy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kmdmwpml.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vhnjuzxk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2afljpadq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2hquucneb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ztlzwsta.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2cuwonnft.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nigvwwre.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xymiksod.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lbfewwge.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qheslakl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zthofucx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hgjwkint.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lqznelnq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgxcqqwk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uolivvvh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2flbuwrsa.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qedhxgwi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icaodqbm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kissbfmk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iumyzdqr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2agqvzktl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nzhxwabh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2krlikyhq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xweetmvk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2eoswjuqq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bflyzygc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iahomann.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gyadrdms.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijxjzcqy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlkgqrak.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wutrqovo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pupfvkhw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjljnhby.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xevkoqwq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbfaeqnx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfuvolnz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bttswmsg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uizdxjyc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hkkguxog.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pjertfym.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vmshpcqf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2azwdqmwc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2unuvpoht.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pnwkjeum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2estjyide.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ckfyodbq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2abxdvdur.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ccqqqsdy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qnpawisv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hpwzeqrq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wzaaozxc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fsfezazj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmgwuxkg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fqmhgpvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pepywaxh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qfovoebe.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jxleeneg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gabbwomk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xjwuxtul.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2nxofhuqx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqtutpci.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rowtrfre.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zcgcmctl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nwzvdgqb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xbubveze.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2rwixhlca.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2umlysxpj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2npifcckj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2smkqtsct.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mjmrchhz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ticbjqcb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dvloilki.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2etbvuscq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gmpxrmxd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fnwfhedv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lsdqstdr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qingpmks.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nzotbkil.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uqupbqkg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vcyrnaxz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tbtgcdva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tkpbynao.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2avpuygpp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pxjsiddr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiohndem.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uissfvbi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ceeozxqd.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzdwknwx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jeistddc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2crttangc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2gdrbbczf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pjapygqv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xxffjbgw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwqcxxjp.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iydmefju.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yfqvifaq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qatrikmo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2akoypbkw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eoijdoew.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2sjaaucqx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2stfmpmun.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2igjzrcsm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ubsoqzvg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltchanbd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tebdbpqb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkiyavep.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hysqjroi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uhuedqni.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bqevdjjx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ojtyxojw.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qfcjghlk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yflavygu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2onpqxgoq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2biagohdg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2exavsaxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fwglfusd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2sohutlbh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lzapjxbj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zzovavkh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2astapnoq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgmpbogx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2igvodyct.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2xafrhuts.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaivoohs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2usovyvaj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwvdwkno.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2trxofted.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2yxddmwza.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nctqcltf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2hwucxqcd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2akipmkya.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2couvrzzi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zfzpacjm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2dhiqqnaw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ruxlsjyb.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nbolvsaa.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jovuswur.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2llsbqqyw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2pttrkzpr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2efgqvgru.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gbiszhux.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vkonxkrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uyehxybe.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2taxzmsms.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qviwacew.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wndbmzkg.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dwbzxctz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhmtsfjm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdsdksmj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edbydbzl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vbhqfjjm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2invvvsew.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2qjyktnst.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbmzqwlk.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2rpsmftts.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dmyxgqcj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbilyarq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooioszut.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vznbyogu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qpuqvwdc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gpxfrhxf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hbyuwnbs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vvrbvsky.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ocgxtroo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2sitierxx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zskljcbk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zaqtavjl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zqzerheh.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nylourzp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2haxgdxxp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2lssdglqx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zcrcvxbi.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2snszotwq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2efmaztay.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qwwktiuc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kfqkrriq.html


<!-- 参考信息 -->