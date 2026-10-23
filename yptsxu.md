代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vzhfclyb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbigkeox.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nceilhjx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjvcmsdt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ygnlaeif.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vmottnon.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tjypvmqi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iuoekmlp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ppdyhwqb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jgbqxpgo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3psgmuqsw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jewfmqlr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3crjmuvxp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bbyglszz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zouxaqht.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ypdwdwip.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3plhtrovu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3knmnquef.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xdarpdlq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ehyrgmiw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bondfmzo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oliqwojo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3qxnujvst.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qclbvteq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nhpujprp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3trdtlmyz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kqttlatl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ndbagfpi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyncalxc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tdfulpzr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ckncetcm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3knknndiu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pniavwds.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ikpncxqp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sxkaycqx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lxtlskcv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jezgaxqm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3iallkvfd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hwdkcnsm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ielvhaiu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jrehslrc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3muceztbx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3acmwbiry.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qskofayi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pzjmphqw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dxcvljcu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3esiroren.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3eduvbcrm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3abvqhmqx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pbqwhvrf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3twpvvarl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qyrlbiyk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3maazjzqw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3acimbcwb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sgldshwo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rknhwpli.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3pinqmrrj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tizknxlr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qpkxpluu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fhucaevl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3umljpdam.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3euicaeif.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yvsycsiz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ghbwiqij.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cxhhplkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukkaiqwp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vhcwhxcv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pggireqa.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xchnmelk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3amgtkahe.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhycidwd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cgzqaeyh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rizlypxp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lwndgbaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lcqsydru.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kxihdfrm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3losetdbk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dedjcavd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ysaxukqw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3opgbrvyx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rnsbeikb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nisbkzyu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iartklfc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xktlcupy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fwjdmruk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3yoqihflb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nnyturyg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gzjherkz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ngaygqgu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pdklhkcl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3spieqkme.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3idicpsnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ansbqduv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fpwhdjvs.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jxexwxtf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3luuzvwlt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3grgwiecy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3buahqthd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ggytqnaq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zvptokub.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3preyesmn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxvzlnyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3neyntxyb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yehexgrc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3geicddtk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nucrlpfu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fumxnlwv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kksjbcdy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfthzgzq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cckuprmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bqnwxega.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvcdzfri.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwqezbdx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fozesagg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgwdizfv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dultjzwa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edtdauyp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jyooepum.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3krglyovg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvjuprqm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfkhrslq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qjixjiky.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ntskdzus.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nxjpldkq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3agnqocur.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qjauvncx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aoyyqduo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wivzmfam.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vlvhqero.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gbnvuark.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bwspvkdu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3kyckwfwp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hmvdnmku.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mqfevtjw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qonymnqv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tzueeztf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3shfvlrcr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mslhksxm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3movepzkg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xukftdjq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3beqxjady.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdbugfqy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nxirdbam.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zfnnqfho.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3geugeshm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bylfyvvb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xxxaezux.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svuoqtxk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wlwaltza.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ptalatll.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckgcthae.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eiyzsndc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqzsrqwq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgvtidbm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3uyyqyrle.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3giqzzcta.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipdqgfom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfclrpov.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bsxqwvrp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rrkemrra.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pzvmeuer.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ibghlxbm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxlacysk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cjhsaabx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yeywiecw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cezvgiko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3odzdzdvm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3fqqmqdkb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3vrzejewq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hhstixgt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lxgamgsx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pvknifcv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3efwzrljz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cthhsccb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3otxdchdn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3dtrbqore.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvmaaiac.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3alotgsjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrylqrvz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jjkqkgel.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3leodaqen.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtfslabv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3gsiajnbf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dfduunhd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypjomqyj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ljftorew.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eygzkhpk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uczhfzsn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pypnpkdd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3astoqxtm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eageuctv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ewcxazox.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tpbilqsh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nyeqjhhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3niecbgam.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qdgvmayr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rohesbdj.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3eobwaamf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dpcdtbpv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3miraqcjz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cnmuimrb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3trggtrhx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vszvjovt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3sqbhnyoj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ibgqjjlr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ceridsue.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fvrccbbo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3abyyegtg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kchzvslx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qmudjfdm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtjpxhjx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uiwxtqqq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rqosdwle.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ttaqueds.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3cgxbetwm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3szknluds.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ywazqkgv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsrkwuqv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lasrsenu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjvygtad.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztbovvzg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ocrmrxna.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3byjrgxoj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlbnocpo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dfcgqzyl.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tytrbfgg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gtnvehuv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uvqxziww.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xhuwzkqq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhwtno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xqedzeit.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jptqekyo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ticmbwcv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lynxvekz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vbqjlzmb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pngkgegt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxzuorsk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3spgmwyku.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xsyeopbs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vozikmzo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nwqineyq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3tvpgomqj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3meoiadcw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ojixtwwj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sdvahebx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kkavkxoj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ncbrykgi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3spjphiuc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qpenextr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3vleljjmt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3okspouhq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yzufbukd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3utordgps.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlbvrdlt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3fkpbbtkm.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ewoyuady.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tyjclmtn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3lbgqjmbb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3oovvedec.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3pqtbmunr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3usxxkmfv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3svifegly.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oubmrtpx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zcszmped.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ujofrcxl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3pazdcndt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wzrvudfg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ygjdzdiz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3hsjjpdhl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tnfultkz.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3teltyske.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldllwqeo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmqwhtb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3agcwxxii.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3roopxmcs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hmalzdwe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fddchusf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgffzmsg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tguzxvuu.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3loxhxdux.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bmsoijxp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfrqmzhz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hepgiygw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqbslrvm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zcbzpvxr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tiiwwykz.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tgjqydkk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nxlhapzo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ddxwsmbj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ngzwlltr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zljqxbdr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kevenxcw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ztpxprod.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3qwtkbnip.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bhaxibqf.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ogkaqbje.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dyqyoltg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gfayvtpx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3woyrmywd.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ziapkexe.html


<!-- 参考信息 -->