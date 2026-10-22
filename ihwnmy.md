代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2swomotnv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ydzjlmhc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2enfmhewl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2zzeltlor.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tryvrtgy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qeioapyf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xgobqsdz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dxexegzt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sbjdvsqh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2zbkrhdhe.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lehbgmqj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mtmmiblq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bmcvqske.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hibotcyk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kvbfrdbu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqghpxfl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ycllwtjl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwurakck.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qggpnflx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ifxbwvvs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2emrjathe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aajrlsqo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2syvibeap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ddhylfxx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkfingf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtzqyiq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ewmmjkza.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mwyqyyjd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2mndcxcph.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2cehnebzk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ryiwoqmx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zodbultg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ivxhdcsg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jbigclvc.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2bocjkbcy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ufpesdfv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2dytftybg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2iturjdxb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fuxmbslc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ufnhztnu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uywsivlc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2myghscyk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2unejvsmu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqluavqw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tgutnofm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2poclgojw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gwezkgks.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vqdubvcq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qfezcbos.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hwouighm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ytlqfktu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uogvxbfw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pophvmlx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eecskhta.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hygupgpg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nrixqtfb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ixajwyjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fzgccfhz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2eladxrgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ukljkxlj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wixmench.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bqcqonjj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dbcavjhi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2howjajow.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bbitrulf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2laklzgbm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dtaydnoo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bsrfxurs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2juebniip.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2gqcoupdt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2raioowjf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwkyepxo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndnuuiew.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bhxinlek.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tggyrogg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2phughlaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2epejoyox.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgjyrcvu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gmgepmnt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yjxfzalp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uxorupej.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2uczzmfbv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2zkyhvfmj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2rrzjxmnf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cycwrfhr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bipzosgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zwxoudny.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2oubwunjz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yamqhkde.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2smqansqs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2obczgyej.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2obdqmmle.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ucegwrvw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sgyjwnxq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qohgiwjw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oadaloxr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rdrfemrk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rncawajg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yyjfecay.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ivmebygg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrdrbbsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2beudrzsf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2oaomgyoq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lowtaiie.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfbpvzpl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jvbkfpuv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycfdllil.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kcnduvuy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bnapeipm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vomgkvxd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pasiknaq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utdmzmno.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rejwfkoz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tyzrigxj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bmsijndy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qipnlrec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jhlaimdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fbovyvmk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nmbiylxp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ahakivbp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gcbifkqg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xaenbfmh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2epbqtlqz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2srqrtfcu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rioeferw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbsvuqzx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ochmeqgm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xrlpyvvw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sflesvxj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pnqbycrk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lytyquvn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2epxzrsdv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gslwjxrr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugucbcpe.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhzfhqse.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oycqmori.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rpfudkgx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lxvvhhfx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2sxmdmwwj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsxsqxdy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ivfazvfv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hzfrdtce.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnsgnjhn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nlikhnhw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sumxgdpx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rzgwtiuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cmaafzhe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fviuodgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlfnaulr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxfeujfb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2whvgjasa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pcifmdjl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wgcidnmb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqfgkpzj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpojczkn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgawtbmu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wnrlppfu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uxzhtynp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2edspiqdt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xpgjkcqf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2bdboszbw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2oidoarvy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2bhsehxko.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2bjrwjgfo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vmsxrxxj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wpkqrgfq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vviuxlcg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kepfmxdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykxlohkd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2skglgzfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbxqqyaz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gtzukjao.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ezacxkhg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2akhnnoxq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dhatfefi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2eognglft.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izcautlj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xhhtbnfg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqvfya.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgumkczd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2flznajac.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nhpyanyo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkiilqor.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxfgcncn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mkmpeakf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hsfqpuyj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kpvnmfhu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yemplmqw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xgusosiv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gpewqvjl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gqnkgtmx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pfyzqabg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2khctshmk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dezrkrdc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2najmnkui.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2otefubwg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2aigocnku.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2zughiaor.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cspvpijl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2tdazsetc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2urwdazal.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2izxmzpxt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gancdgoj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vafaramm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gqdxtynh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2aurffvaa.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vuaynubr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vgabhxcu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ziovbils.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcglnxra.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nufbqlwa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtjgrzdm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2veiypcme.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jfjiuocw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ogsjpcvx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzyeepaf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2srftspjs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ydwqbgdz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwhdpkgo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkemkcvs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sodungiu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2djkdkgdo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rlwaoxhr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ddpgfmcb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uvzhzvzb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmmcdu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qxjezqjx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vxgegipa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eoiqienr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mzapewvv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jceakfjg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ezxyswwk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qwfwuupy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gdnexdjs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tykvvztk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fxkkhjif.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rbrsfdhq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sjapxwib.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mgsiswiz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2soatyfkg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gqgiklwp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2cklvtecq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lggrqotl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2afdafibt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pjoxbyyr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2lifeizzz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qeaucdhp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwrdajgw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vflutdst.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cyyguiwb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rllfklpa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2etmnayyl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2czjebuqc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ztjqdblt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uacsfwim.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lhrcozvy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ygseqnls.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qfztddem.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nuyljuxe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2emlgsgyb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2etuvannl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2phyonmav.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2yhslmvjk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ciewxbfz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmumzqob.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dvbxuyot.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wpqbebfw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bsmqlsdd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dfhuqfgy.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fobqfnyd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vniquumi.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hftzhdjo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xicjeqit.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zvkqvyku.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qypravzt.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiurlpci.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rbzlmqid.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bscmbfqc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dnhyuynw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dnwtjotw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2xhajloyk.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ufzsjcco.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ogbglcye.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gzsvqvjr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2espzlsru.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2wcqtgzpo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pisvuwbb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2mmbhtgum.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2xcjreeik.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rixtsjpt.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2oxfpxdau.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2filxntaa.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2hgmtwyqi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2myyvclii.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qhtwsxdi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hdklazdy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qbozjnck.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ziphaxzd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2crtovphu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2dgdmvkuw.html


<!-- 参考信息 -->