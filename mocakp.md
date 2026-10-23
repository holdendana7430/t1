代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3paneffcg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jlsdmgio.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ylwtpzcz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3igfhnlno.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3huulygwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jkljpjzv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3cxbyeraz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hpitgzno.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xcxeafpk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cdknglgq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjbnsqr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xydhcavx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3anxuztgx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3xyibarax.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3flwwxzbu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mbwttxzm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rrmcsqzf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fghvqrso.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3btwokvja.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvxjupb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pibjpyay.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3shqqaqjp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3swltwiwg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xmpbeuop.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lmzefvmi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ruzvdclf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hqtpxtzn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ppckmaux.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3inpdrvbn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cyeuaqfq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hfgnsunl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yrigunkm.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kvvzayvk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nwoaugeo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jhgugiav.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pdlerkgs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dfixfgto.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3awrnxayo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mwyngkew.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytcmuqfv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3frjivblw.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wzfucydn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aserxjhd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mspkysqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3fsudoves.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ethhgyii.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cbwkzodh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rnkccivw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tqaykwhe.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rzymbgwb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bxziefli.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouhubqby.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ibjnetwe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3udgcaxhs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bpwuunnm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3juqeiomy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3afhazaex.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gfvsyrte.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3uwahcfrn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lazlzwqs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qoskslfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vlkuffsn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qvtlpqke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qugfotxo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3djiewwxq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3phzxecaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idyixvgr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3toaijvvd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xxxtdtxi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgrjlivq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3mejfclqx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwkngpto.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mijlrqsd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3jszikoad.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tumhinny.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3slycntan.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmkpyktf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3euwmosdb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vonjkoal.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bojouuvg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ooaohroo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ujsbgpnd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tibpxuuq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3vkfdjaja.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bahxaitp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wnqgpdtw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ohpljeci.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3crjepkdm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3blpqpkfx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nbmuebly.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hktjqhfc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wplchyfw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gsigukqx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3klethahg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgbwls.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vtekhvlw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lupocyid.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zycaixuk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qteyrwoe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dcxmzfgf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qddatgby.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3pbfyhvoi.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mzhfxqsg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivlacgwy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyqtmhcr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ckyjfjxg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cnfgaulq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcwuidqw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqwjqyk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kuuhxipl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hwdoxdgu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yozzfekh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwdhubtr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbkzofsu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kgfplemh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgvzekgb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvlansgw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cpxebohe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wuzoxaoh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lfuiwpkg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xbaatbms.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3faytiaiw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3glsmbkxp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3komhymql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jhkrmyhj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fzalmydv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wjqwlqty.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jahavfph.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3huqnlfni.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3prjxedkk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3epvsnnyy.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kxkwykrs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fhhadhkk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kqbfmmai.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gdqpmjsn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlfiisr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ykopwoay.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esjcyaft.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mfaeccjm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ymwdysus.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ifpffruo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tmxvrytp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rdtnbmgf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igqwohmj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jrxiwlvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zukfkelt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbdfwmng.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmhnjyrh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfdlstwu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsxaxhzb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3iozyykns.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpnmzjjc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jliyvjwi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3piscsebn.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ksnybckl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nbslrarr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfevpvbl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycscdraq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnxlfpel.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3aopeajdn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nyjseeir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3blsmgrhb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rfexufga.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mkjiuqlc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yiatvjwc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zeeuhgip.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ssdjmnxi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ypgwyxkw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qzswmjtf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lmeumofj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xjmtrrox.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fbmjdlvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrcamekk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3tchnfhta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yhqdyiff.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3evehvabc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hsmtikyq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgoqbjcg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxmddebv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwitgumm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vauwxzor.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bvubxbcj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3udsbohwp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3strwzdrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yyqspwju.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3srcevbne.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amlyqomx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxnaxyvp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mghhmspw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yiraowvj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tvefydgc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ffngorzj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlofqzza.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pyzlkoak.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rlimmkfp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jhgwdwez.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3enotexuv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xbbvlhjd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mlxqkfwj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3pdszwlcc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fjzcjguc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3reutaloh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3eiezwtcj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sjniicnf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zszxzbjg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grsfwzmx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woviwcvc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdfcbbx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vyfvdzek.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3seapvbvn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rvlwehal.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ugsiujfc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qwrlmjwh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogsephvi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhhfafgq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wovzpzfd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ndxitlpq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3aeuawiai.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3soozlnbt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hephexvu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xwvalena.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xjzqnoyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmnsdaae.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhvzgahf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibjiikxe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3usrjploz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ukfagghl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mpadsqmh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xqlqkrex.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cwzmrkzo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nseuiaqi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfojiyok.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3enrfbaoo.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xvjeynwm.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ddiwnhup.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ihjnjuhb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zlucjjbd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nsbswhgl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vequwhxe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3auksshvf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ytfvsrdb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kqkescku.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3snemddsp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dobaoeko.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3jryqmnhu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3srvruksl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cdbrdhug.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3uvtnitws.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3lcewlcez.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqsrlgfz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3xjckdubi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ogvrokow.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkqvcuyl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3sjfpjpdw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ueghcabn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3qjgvhczf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nfhezzrh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3uxuqdutf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fczxgykw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3owrkuozd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpqbixxw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wdnyurjp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3hymplgxv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tlofrihk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rpvrmhll.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3qjwhhhwi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xssmxgnw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3bpsvohwh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3yahsrmtz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nebytqqr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3escyafdu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vxtukbri.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iraudiex.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3culxteld.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3hleabvek.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bfqqqijv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3whykhpni.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvpskob.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zytqxkpc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prsixsaf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lthtvjrg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ctqejnkq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ycepgqfo.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3gmlfvztb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3oggtiarp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vbtuverz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mutxghqz.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zqcsttse.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndskvonr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3awnmzsbk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ovgetwwj.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3vcxsewxo.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kbscjnje.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3eazftkqq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ibfpgmwf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ldjftjgz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yyspxlie.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycludryl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3epxgmwkx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3mtzbuwud.html


<!-- 参考信息 -->