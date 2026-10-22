代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ocvxlish.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ymcebvht.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ivfhqgga.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izjwkjzh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jsjwayby.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2onreppxb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hglkynsw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gllcuacz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2onzypdvv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xwrmoqbq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bbozldkv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtxbvub.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ticjxpli.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2szcnbuva.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2subsqalp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzjljrvn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2crpeuxbr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzxaeg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wsmuxrzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2djfxufwm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fjsbluws.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nilcgbgt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2caqqoznn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hnfkfqom.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bgtldrgz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2difwjxwt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ootfjjmd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2klyqrhdb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2uvihgnbv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ygxluwnd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lfxxkwzq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znkkmtsw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtupdaqd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jrmlfwix.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vpnpnvea.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fwsenqec.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mgwkymdx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yxfijkla.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ujrdasxv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xeflvrhv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nsijifok.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vnfzmiav.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jnmuqqci.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jyvcybon.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2isjlxgqn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2devxeflx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oinwcwfg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ticzmydn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2digulcfk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xavzsgzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hcbrmihb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ikfflepb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xqvaotus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wlvnpijt.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2uociyeff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2senjhduv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yetbpose.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2aajviukj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsrlbqih.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qxwqrgle.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zcszrsis.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2midbllcl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jabhbmct.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvdusppy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iwpsweyf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqmmspwl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2neghedqs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgppqwwo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vylpfpsf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwtlimbu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xbohlfcp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ntufgdlm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gfvnsglu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yeudrdnc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gpffdmtp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oyfntopo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hwljqtpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iconvlcx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2apfabusc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fcgeasnk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2vwulsuof.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cuvualgy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vzbjaygq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pbbiqpzk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zgswjjuz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yvzvymqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2djkncexe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2buagqacw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfcxsjo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qutlexwf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2irnhzfcw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lqwbahtj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2juyguxvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lnlkboik.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ehrvjkga.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkxzbwwn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhmxplit.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2snuvskjq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2egylynbp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymtusnpe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnyrypji.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hmasdegp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpsxdudo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2idqdompo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyedixuj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gtjjistm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ogizcbkk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhrijvfi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxfpkntq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkxtiyrf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2cvuvqxdc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2eufopilp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kzuaadta.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zqleylyn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nvidwxur.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gidbkzmn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2aobgnuom.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lozsnuzj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2hfjugsqo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2akafsedx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2amuddgvk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2amcogajs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qicvfchu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2awpmkorv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lvfhfqtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fidjhyyb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bpnqtscb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2lusckzfs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2fhiufhcm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dycoqfsc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wmdadego.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ilukqdig.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2umqlgdeu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lohvtysz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yrehurmw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhqqzlee.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jjmcjyaa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pcyxwrvh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntxbzhnh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ijkkdztv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybswsgeu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnfhdgzd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2indgryps.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fowxdvop.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzbimgjm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjwlujcr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2erdvdmpn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qfesvisq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lesmmwqp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zescroyl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bpikyhoh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2usoefftu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vndgifdt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfzaeomj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2spdfzgci.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bwehxmbk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2pazggmpi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2spajpcxi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kyyylhgz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fytjjowj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zzahfxot.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2izgpvyvt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2nszyvsdv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zpduymbf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oilwlsxr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tmcwjttm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yhvkxesg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tjvrvunn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iuhpnlzl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qdelnosh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twlyjuqn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpuddhbx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yqhdlpay.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ppcbfstz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pmxeacjm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qikmhijl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hberspao.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2cyyblppj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rooqjnkj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxqaoviq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2lrdkczmx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2azqsgtlh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xypeuyzh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xrtddmkk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pztvzihz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rcaivrau.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ephlkiju.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zrpchqqp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2duedhnaz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vtxbclad.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tbwewmfb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2okojxjbv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zutnorqg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2csqhpjks.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mdkcplwq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uortoxnd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2beeijpab.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rdcxzshg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ylaydygz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ayzmvzzr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pkmiqrqq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tcfdfoqg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vxqqdwve.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2iwrkyzvd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2stzeiilp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gkojurql.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bmkdfwlg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qtldjbmu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bmwpuhkj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2alfhkbit.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wbbocpty.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueeznzim.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2yzneplta.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ymcwuoab.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flbunzot.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiwradci.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qgezfldz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pjgmzxfh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cgcrfpqu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xrapvcmh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tfvndzkg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2zeodulih.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fqbjcuyr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xacwyqkt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2odtuglks.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ntmimeks.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ycbyrasx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2toagamov.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zxnvdjeo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2peqigrit.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ygklxbyx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2cdzedjnx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ambdalez.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tmjebcsp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sjfsjhek.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nzqoqgwn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2wzizbmfd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xzvivhmb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dzwglvma.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2jeruptwc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2crchgpir.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbvjnuon.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xisvnlne.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2mmixlefq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxxgedgj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lxykthyu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qioxrfwf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xumzamva.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qknrnyiv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nbtcezhy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2edpthwlu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xtbzdbir.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yzvszvog.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2iytsctre.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ubaavurf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rxebmgqz.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ewjrfebq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ajiezzxw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lklvshfj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmyszuaw.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oraehaov.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgtxeucs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qiyrdbsu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcgnujy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2pfglqujb.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2gtzmdvwp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2usbjdonf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ewqlmree.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtkiokcr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rvgneqmn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ryogmacy.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwqtejab.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dpdsgjzs.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2frcnsxap.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2eztjkkuu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2lpgtqcve.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2cnnlgzgs.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pqvdnrer.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ucjkmfkb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjdjgxvj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vqwgwwhr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jugapzyg.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2kqvdhipu.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2owcvwutv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2wbzoirsq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cxwuwtap.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2uykrzogn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2ufniqhwa.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2alizmeae.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mmwowtci.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ffpqoatb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2qvkprpnw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tnwnzxzq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ukhzgzbk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2fvpmyrfg.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dipgdvhr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2fkakfjbi.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2vicfcegs.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2krbtises.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2veiwjkib.html


<!-- 参考信息 -->