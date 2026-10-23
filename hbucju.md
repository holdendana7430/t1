代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qkakcwad.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3urulkgqz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3aekrfrfr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ivqvgies.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3lyowaxbc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dzgjsbxn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kopezqvl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yjatzbjf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqdmcouq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3anyfieha.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tzgsbgfq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kazpotjg.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3efxhqfsd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ovpwnmzj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wbbczcqz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nznodupj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gtdkxdkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zcytusdg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hihadkdn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oihhltqn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nqosgwnz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ercrxigv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xeaulmgk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3difbrrkj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pbsiuzpg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kqwctnec.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ahgchret.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3evaksbuq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3veoyoiwi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zsnivzjy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fedwjkqk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eyghlidu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mcnjjzvf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3abnysqij.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3btakktds.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghmqktsu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3dlarbwxy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3iowxjjwk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uetrehbp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ybikonfi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bufooarr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zymflamp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bkpzalbo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vluguqbj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfesxgra.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3sxizhtru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wdwyqboz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tqwyxpcz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bdxbpkeu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjvqxqh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijwufcrd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iaenyfot.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3igetxbyy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wlzuutvp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lihnvoyk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yqtjejat.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wzcqpbee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twlugsam.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vkbhthbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glxllfbk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3cwrupunx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vudvknsi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tacklcil.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rcarapvy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ajndwexy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uswasmml.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tacssvhr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcyzoflb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sueqmsvb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kqgtaxys.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ashaazvp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydtywnwx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qqegqekw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xrafjumx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wcxfygfl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3khgdauvi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mrlfffso.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lnrzolik.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iblydvwh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bndfdzft.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dxejzqng.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rtvppkut.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mhlfjgbv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hvwtjxpc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ypsbnijx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3uxtrkfmk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ggzxjhpe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bngyxevi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bokfvrab.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3hbmkgjpd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3chdcnvua.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hqfcivtp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ipmwnesh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iccajssd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zybbfkct.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3etuuvtpn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vhzpxyus.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gbvpngft.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pesnoevg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwhkvmko.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckxtbakm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jvwiyfkh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3trokqzrz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxpsrccr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxbgjbsr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3gpqkmicr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flsjychc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qpbpdxfr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxfmynhm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fphgavym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ywhggzjp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvdglccb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlzspgdl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbnoyaef.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hufosoro.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iwxfasvu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3izkbwurh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wvxgdfpb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bnffzkhm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3aqvhfqoi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jgsfveym.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wkwohyzt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3enaoitfc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3luzugvzz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ovjqndwf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3okdfzioq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sturewkt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3clumqmhy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3spofcuyp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lbbustiu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ixblukom.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wuvupuly.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cdgbzqnz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btfibyke.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zrkyvgro.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3umosgnqn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ezkhaprv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ztmqmzci.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mbvsqemc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iszczozx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3trrqbgxw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zhwmzked.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fszyvefe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nznbycqr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oznxeodm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3egfcaaui.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gsyqyqbf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3krltokmx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwcmqhvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enarucex.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jkzhhmvg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbfcasam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kagokryl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mldwemca.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lttdyunc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jjdoxvdk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jbavjnpf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzlerxnq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mavswsdi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3elcudymy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3xznamqua.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3kbojczhn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zxwwxpcz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bwujjtmh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nrbskfwu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gukqaybj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3maphvcyz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3eoqqzsoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvpoyfas.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ogcfkjdq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dimfaypm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hfjwvjsp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3djjbmfwf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iypaydat.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uattwqjg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3npsomjur.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gmezcvbl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rwlsphqw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sevysmly.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yulsjcfa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qvukbjuj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vyxspeos.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3kuvjafyp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgyvokwg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwssxeiu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mvlupqac.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3prmyhbzy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3abhkiwns.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhmuugor.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ivcmcszg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cakqkrpz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wcsedzri.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3guwyzabr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hyfhuvfy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3toresviy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3onvebtkg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aoceemph.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wvjekltk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3scbxxggg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ddiyodmy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcmhtjwi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sgpuwfbi.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jurepwai.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbkarwki.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3moarinbs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tncafgqm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ozkxyozd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ximgiebv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3gnltdscc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lbsbybxd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sbxrsjgi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqmdltlj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytvqpdga.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qmibaday.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mmrdquey.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyqejxkg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uhqczlqk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cepbsjos.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3plqyvoze.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntounnfo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zujrhleu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmrbopum.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3splkgpkg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3nfrgbssu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3lfqlzvsq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ebiqywcz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bninynax.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tqtykxuu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yzwpzgzm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3flvonedg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vuczzuru.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kaiokmyt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gkbmauax.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ujnfifky.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gajulahw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3erdwpnda.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvbenhfr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3znzgljyd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfqibsnw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiogeimx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3iwwdeyww.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ragtkrdx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wtibgfdi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ergiffbp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jomnibvc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3agjcxond.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uhjrqkbs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybpoahji.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ffkkkwns.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fxiyrbis.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cqfdtrlw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtpapdwj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3lcvnuqpd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hwvrdfrj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sptkxqwa.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kfmznvhv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nhymwvsi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3qrtazvdf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dylyhfxj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sgsrmdcv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gxnxvmpk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3zevxrnfs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3taglytvt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vuredvjh.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yyobfhtc.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cehrtteg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gilgogxg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mmblrqli.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iqiypbsm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhhinytg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gkufzqtn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tlqknphv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejadrilo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pscjdiag.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3etthmpcg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clpulpde.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ozopjuhu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jmwbhotr.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pmizzjdr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3kkdulqjh.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ubjppgqz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3chherzrb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uzyggmvb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xboklbni.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3zeqrvqlk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3mjxkpcca.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mpegxhvn.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3maaounlw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3syrlruhv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3gidebpzr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fxvhczcq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eddnqxcq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3jwhhvrvf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3scdlroeh.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcdgrkz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3hkbifkql.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wdnangfc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hnpohwpv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3evessuqi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfshxjpy.html


<!-- 参考信息 -->