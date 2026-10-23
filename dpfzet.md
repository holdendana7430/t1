代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3okeffxbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tmodhfce.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3oxjgjigi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qgkpxsoa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rqdrnkxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flazvkid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fxqucbux.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssllyweh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3iokkhwqs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3sluzcbqi.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3whpxwnwr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lzetviic.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwnvmyud.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3voqgmuyt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zhsqetsm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3esgnqdwz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gzqybeqn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3avlitimy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3reoukebs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3whazytds.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3eihxseau.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jqrsoeuh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pjamkovm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dixbswkv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3neobeudt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3thcxomvv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3syhiyxrv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3citlyqxl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ufpegfod.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uamdrppb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3iqpmcdxo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xgwbtqjl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fhezbpws.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vkpayyia.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3imcerpwo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dfbmrhoa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdhmumuc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ofidbuwn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bbahvxpq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lpjoitgo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3domvarvb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wyzonsro.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ajmowljo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ytbmsisj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eavkbjem.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ruhxyfgo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aoytihag.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lujcpzaz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3tqejhvne.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ahavbovl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3swlbamxo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ebphjydn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dpjjfaal.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rmfviaeq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kgzapybs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ttdqnqvu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3fopdmamk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auweyzne.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qlgyezln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fixrliih.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ppzdxkwq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nkuxxpao.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tafpkygl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ernnxmvz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ztngtved.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jteimdjo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3rewatvzo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbfqnvet.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tmibdlhj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3vhjhemjc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lrmuepko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sgrrmxsp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cpqijbxm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xdxqvcdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qjoogvzs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3egwmyrnr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3akcdpjcr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wjkmxgft.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xmcdqmsi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qyzatqgc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3usibetgl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mikconft.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yxwpumtm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3omnyiuzb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3aorgkkey.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ubhdtmcr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pqywotxh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwjrsgus.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ecrhzafp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3uylgxkhd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kezmqyfj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sylycbkg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3tlqvjrbt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wgmxxkys.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cxvjgrtd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lqukgids.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fywaprdb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lbwncqgf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dgxkhfof.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dyltblkb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cecebsxq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nberrqel.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3htmlriyp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qevqhgja.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqtvewhm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xddsyecq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nmmcxnji.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rdyvsqkl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmhxwjnl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvytxkrb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3upnzxbhd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mfjqljkn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3koygotkx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stbztndm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mbqizdhp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3muabsvvx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3apjhkxjm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3yqiyuwte.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ldcecfct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3couvtflx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ghxaedhq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3jepvamuf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cncafiwy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dsmjppsa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3eoqejdbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvgzhfae.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ssxwfzpq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tyamcoeg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nvegluqw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwcjpae.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gmplcivg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bcbqujig.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3klivgagn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ajwnyqpa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkjipsqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fztwbodj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mvrkrtnj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wpryzpyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vjkqyhsu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3luxjooxs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqjejgyr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3yacstiid.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lncgnwku.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3htosntco.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3razpuxja.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eruiqmjm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3mqewjyfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqgzfkhr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prvhvwtd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xiuqcfuo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nodqintb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tcqtkrzw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3egptwesb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ditxraxa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gczedqok.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fivkytmi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dunzvnnv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxbiigbw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3thdoyzgv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3iufxjrfx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wkcpvvlk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zgvtpcjd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mfekeiws.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3omdetirj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gktshfdo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3otrweprv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3azbroizj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vasjvjxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iixhhbxs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dhetubzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pbxkmuel.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3dyvmnrid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3rvmgvvyl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ixhwrnsn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wufbuvoe.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivfhhsqr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ariyiaiw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3clunqqam.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nqtyahlr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsiiuayv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mryidmvr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3trphxjbh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgryzzps.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykfahqhi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdvvgoqc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqdrkrzp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mdyvvccn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vewjjvoj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnbkteto.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ncefssxl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3juvpdvtu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rghvzuoy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eraqznyl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3stmgedhf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wgyaccsi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pizzoiqn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kjqbfkzf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wjmlgvbl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3sliizetp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fgovekxf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yvjvgrke.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3goighstm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nviqkcdq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3azfgwfsj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bibqotmp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jslhlrqq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gjpcgpzf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3updffoqy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fqrkbejw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jhjzqqcy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwnyibxk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqnprfom.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdhkyicm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nhkyrytt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vqilndlc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jmzmtmct.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3oxnaaylk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mccykmno.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3osocmbhu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ysbeaynt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rclirzoo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ponqcrsr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rjzrarsf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ystcmsjs.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3bxjnbpqg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fqglwmbi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vritmgwe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ofmbgsqi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bbwynqkk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jxlodmyw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3djkqhtke.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dwwchmgr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kknalzua.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ymklemrr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3pwdstbot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gtsghbhh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3xcbyiepi.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uftxlmbi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3adkuuriy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdioognk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bnfvvchg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3eytcvlho.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzudcjrp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jumkymjf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ylbipokn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ejbjoesr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ldmjjnus.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jbbcbksp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3poiwybfu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xrbqakjm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zhmaatbv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtvaaqzo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3joqhoxso.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zlcptmtw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rknvcshg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3krymjorg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ftnxuskr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3tgiewxvw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xxqukerd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hsdjoeci.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3zbxfakse.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3qsbkvpxr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ukpcdkgz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3izvnfztr.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pbbhuhmb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sihxswmn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kuchbyyr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3avfbgvfy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3szfjehvm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3uepmuirj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyeybznl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3agkubfda.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cyisbgxk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwagyzvq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3svdkawpt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkzwfskk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3admlgsiv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3udfrgfez.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3eywhhyph.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3jgkhvndw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3axvtzwah.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zmkzxscx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vzonqqtd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ekxnhmjd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3epthqzsh.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nuenxjzm.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ozccvyyo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3apbikjvn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hkhpnvmo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ibrilfjm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fcjtztfh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ziknjhud.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vapmfumc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybbnrtde.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3yrmsgzgv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tornyxlm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bnmugduk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3nyzslyyq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qanxwfxb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3feedvtdv.html


<!-- 参考信息 -->