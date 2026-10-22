代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vxvpdpjs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvyizgha.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2reuzdkit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eosljdrn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2knvydkmh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eiuoakhl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ixuccthq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qzfihzbj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ekwgttca.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pzoschxi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qjyswbrb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dvurvnnw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gzdmsqcu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pzzjxdro.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yljempil.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mjraiucp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2zgdbjmcg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bvjnxfux.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zttquzvl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bxlsoppa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2foglkkoy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ovyxrpij.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tgvwewwd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2gbmnrrdn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2psjorwob.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lhctkrar.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jeaqszix.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uutzwuhy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2debpvbmb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rkaoxljn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fvaotgpp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szsdawht.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sezbtqsu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2acsoufyd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2wdprubvy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2fwoxsdjk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ghwpesxg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zcadqesr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qjvihtfm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dofmzxtk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wocwbyxm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bnvtxszl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gifobcvj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mlmqoffj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lerpsygo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wndgjxjc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2odrelups.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hjyczaiz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekfunhze.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2icpkyxnx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vczwdptj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ljxnidmv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2agkydzmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvglwxjf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tvtgltuz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pawbxkch.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecbznfuy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2injchljb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2flfztbje.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hjawvkgz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ezszjomx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wzckcfrd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2acijngha.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2riroqute.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jofofrvg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2sejzbesj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2qoniptbl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcspxrzi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hatamzqa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2akjnvrqp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ccdgaozn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2nszcwjkm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vgjglnru.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrintfjs.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2wadrnzmi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wathkhaz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ejessuev.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ifsaarxj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrbzxpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2puullcci.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ciyczyyb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2sjidaoaw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mqulocxt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2osjwsjzk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bwnzohdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2lpatafys.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vecvcbqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ycnnugko.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vfyydiep.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fcnengog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jgjglcxl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ihdctyul.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jnszrycd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ykzrzmvb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdcybbiv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rizojahi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sigvhzgz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jguuemnq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2olnkgafa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlbkyzmj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndvfxxmt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bdvydjnf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sglwcswr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gkqjlqcl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iomxekvn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oavtyyct.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rmrcigyk.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ciiqxnce.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsbeqjze.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mcnywotl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2avmfvdmu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kovfxrzh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2voqlulvv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kkwnrqlw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zdosszpw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2noyjqepl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mafzpoma.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ccwtrbiu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lsniwysb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vxzgmpbo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ffyardvs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ethvtyhs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2viuycwpg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2oouynuhm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2znfpwbqc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jtssfqlt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aqmqwceh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aetepqie.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gykphbse.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rvjmgard.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vlbzdeyg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2quopzvsy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kskuzqtc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydfigbvd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2etyscxdl.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gphknkiw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ltacucxr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ogjnmpuj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akpghqxm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjzsbxzb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oyvytloe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkklxkta.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kjovpqey.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijlphamy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xodwsfti.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxmykvjb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ghqkvves.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbmssaob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbxgfipo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2exshwkud.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phaymskj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2madraxrs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2weabicvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzqhtru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2buxmyqpe.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2akfjfxhe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rrlgrlci.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dougydkx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2atxrerbr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fevutrzn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vdsvpvqf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sptclrmu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xhgwhwxg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2xryfvxxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2voxjdstp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2frfczdqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbvzgoeq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2dexztujb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vubsprfh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yauigsqj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2znynukpv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2srzjeevs.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cytpseyl.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2dbpravec.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2pkwnwqxk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mljdfzoc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jknieyqj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2towfuzvp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prqyjshk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gipjtsyu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbsdmixx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kcvmzlub.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vsqmvdpv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oqekbokl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vepcrwui.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bnnzztxh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uluuekhs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kvdmglet.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yzxbqrcc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xaqjqvfl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dngwqopt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jpgalldi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iirsbvov.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qpzfvwaf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ijoycnew.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mcroapdq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmnthutu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ikhdxsvx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vakopqhv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uqgdpwvf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dtntdmal.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2thilkggk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fhfklsjb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2xtutupak.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xslmrdgj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aenappcj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilxyjcgc.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zkzpbllq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2minpkwpv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2etxcqizg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2iqapvxlc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xpetwiwj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2eibzdxag.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2kjgkxbue.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxtvhwfx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vigqtkms.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbpcwygt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvnzftpj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mmtjeest.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2manohzlu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hqpyyxdq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nkuqpttu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2novxpzuj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mkrgcppz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vskruwkw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xnfzvgek.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tfdamsxt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rlwcplat.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ikxrhpau.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uuqyzkid.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2icckltnu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2invbfchp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2pqasqvxi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qfjurfrc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ebkwhfim.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vazcnwxp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2oymbjayq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwvqxedm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jsdhqong.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pvhhsddp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2swpnxvnb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2baadncpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zddekyiz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bykohvin.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbiztoeb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dtyjgbur.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2cpuovdml.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vtrcwubr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fbodtzwi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pdumyupz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vhutdqub.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zuoryiux.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2msktecof.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gdvkhfew.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2svggrqdb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2npdomplw.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2gklhdpwm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wwsxpjzb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2musifyew.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cvhdfplm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcbzhvyl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxwdqzdj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lxuczzwd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2amybbreq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2kezxlned.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2htqaxamj.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rwmyquba.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dyhkyudj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bnyiedvw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjzsnkg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rychnxnt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgrfsser.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nddpuzwo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rwweaawm.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ijrdvinl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2duspfpdc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2vvkgreqj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gxnkwezv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hegnxage.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pyemmaxq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xeussela.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2smkicdga.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2xnnaqjvx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2zvqqpgtd.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2oohwpiyl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rsmahiov.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mbnmsdcm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2tnkucahk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2trnpdlua.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqdhngsq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2vgxpeqck.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2msslqhrl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pmlbdycw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ostzoqat.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2nmxahkpo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pnuqrwhi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2dhddzhmx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gseghkxz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2unjebnrj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mnftbhlq.html


<!-- 参考信息 -->