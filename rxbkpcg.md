代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gvrduqfst.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gtqrpfvri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gpgxwgcqy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gvnfazine.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/ggajcwelf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gfgborvbw.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/grnzpskdo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gmyuxfnpg.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gyuwsagol.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/ggchkolou.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gsykivfry.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gopsdsefg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gokgoejev.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gutstgrlg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gvbbonopg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/glbbnckip.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gxywgmosn.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/goexzcqnw.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gqskeqosa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gpkpijbvx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gmaunaaob.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gdmpoajmc.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gtfneqvfx.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gtjuoaxjs.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gbctgzmba.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gdknddcro.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gxteowrcs.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/getldswji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gmijxfmvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/giiymbima.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/greltogxs.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/geigimngo.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gqddazajs.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gsajdrnbx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gspgmpeih.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gzoffcxyq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gtwfwkpxm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gfujwepbz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gxviyvpwy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/giqpfiank.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/goerwrnix.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gewpabzvm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gzpvimslg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/goyhhtqdo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gehoaabzc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gnjqehnjy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gzuynmjmq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcrdjquid.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/ghthfxdlm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gthllhayz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gidjyguql.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gisslixdj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gfaptohyl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghhloyysl.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/giebpdoil.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnvhdknzv.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/ggmtmxpak.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/ghrxlhpvu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxyirkjoz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gpnbqgqiy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gltdbgotv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gccwnyeud.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gkzidhvbj.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyuonkeey.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdtywytqu.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gsclxmvxx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gvyksscbl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gfzghddky.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmzkxgh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gcpcgbuez.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/geasznpbu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gbkrhpojc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gdxyrracm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gpfezcsxj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gpgexkkje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gzwjllebp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gofvteesm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gsnlvaakv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqsuxtnhp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/ghqneywdp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gwpaahlqk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gmvtzoiva.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/githspblb.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gquthzkpz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gjtpkgyqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gagcwuxvt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtlmucytb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggccrvjam.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gdtbasczx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gzvkrleen.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gandbrtkz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gvjaexfxh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gtgrnhtse.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gdcammene.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glyripayq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gevwgtcuj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkzdnqjat.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gawpqrjdl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/glushzfju.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggfxjjcdc.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtyromxso.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gltktllpg.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glpbpvfcc.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnvzsofjk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwffygaxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/grbspwusc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjpaspndg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnxthhflj.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gjdfkolle.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gakgglcrq.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gybcwrjus.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gbcnsqect.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gnytlcmud.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gpmpuicqq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/grfsoeyyx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gtodcxaeu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gsouwfgse.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gitfqlghm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gtnrbyfev.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gwegpbrrw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gzrxfzrxr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gcmbtlydp.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/grtnglplc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gqachxixr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmwbyalfu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/griawcuoo.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/giilqhqzr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gjopfvaer.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/godhvfqev.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/guyutrfsh.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gsdiqrske.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gghzxdydb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gispojyfe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gmvbfymxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gkbagwgti.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grnzbszfv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gpzmodfmh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gpajpjusx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grzzasatt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gcszvjjld.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdnzlfvjs.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gslvghmzs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gespyeqrc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gayuryrfa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grgzlwuew.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwtplzvvt.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/guiydcizk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfpakytom.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbntjtvup.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gikssvyje.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gegnppjtx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gxtfpyida.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gspcnhopz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsjoogute.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gjisvurdu.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gbtbmhnrw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gjsisxvov.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gliycgxwe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gqsziswel.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gihcdyajh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gcipvtsnm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gsmxdbnfr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/giraihdvf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gvzeahaub.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnsrgfcsx.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gctddcipa.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdujkuxsd.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gysplmxrg.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/ggvsvfrcz.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gjtwtirmb.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggzigzdpd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gtswvcaae.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gcmofhoxs.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gjyabqviu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gouqpsrgg.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gjtyoekef.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gfwcwlrur.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gpttgrocg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gldrynfue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gtojiywzu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/guivmgexm.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmpaozgtm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gkazftqlh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gpeelqjrb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gaoczllce.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gtoiawydy.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/ggfikgdkp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkwdfwype.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/garwjwpwa.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/ggugntfwt.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/geilhhqig.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gpvevhgqc.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gabuclzwv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxuxiqpap.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gaiukupag.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gdhfkjsyx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gwoobmpnb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gkdglyzwa.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gpoifnzlm.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gryeavgrc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdauwfoyi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gqlzgfhtb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gdxmrjrei.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/glkcjzzrj.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gzlqdwsrn.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ghkdspeot.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/grtkdkwdc.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gcecifwzp.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gayqflkga.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gdbljpszc.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/ghjkkdxwu.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gjzjwutav.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/ggctogwmb.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gxkxpfbku.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gebmlietm.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gglceuowy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gulxocymi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/giewoskei.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gzqpksldh.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gikwlkhbc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gqtijvsoh.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ghahfubeq.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gpsdvjuop.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gfywhhfwx.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gszgrdidg.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gccdikarg.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gmzpkqozs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gyjejljsb.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gzcpbmjgp.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gjxohdpgb.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gvhuwhtij.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gvzvudiyo.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gkzwzwchb.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gcduvfgch.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gjtfdgboy.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/ghetsqafp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gnpevdlqa.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ghsxxaxou.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gyicuampi.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/gahrfamuw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/ghqnppsyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/ghfprxcxf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gckjqeevu.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gvxcrutxn.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/gclgtuwca.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gnhmwcioq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gekajlfiz.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtceadfwr.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gkianywzp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gdcvpndso.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/grlqousqx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.hesvh.cn/Article/details/gxijcremm.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gzoqczuuc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gryxemehf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gsmadmikc.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gqbykcxty.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gdlrxmkps.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/geiwudlwq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gukfsydhs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gthbjzigh.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/grwigphvb.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqsqloomh.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsbjjdhwd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpllvzfbw.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gpqrancxq.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gfnpyfxvy.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gdkqskdob.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gjsmjxpym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/glrieqbyr.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gwxabluor.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjkmqgxbc.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjovppzwd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/giibkvfxo.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gerfwpvgv.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gckguxhcl.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gsxkqxtlw.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gmmyqepqb.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtafxgfye.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggvqzhfdf.sHtML

TS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gjavaatyh.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gkahklqgl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/ghjsddtto.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gmjfvsboi.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gfnuenjws.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gfchogstt.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gtukrfpfn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gylvataby.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/guvgqjine.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gdotccqjw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gqkqsfctt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gpfopkjfx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gpvcuaqlv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/gxobzaujd.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gwpwunbkl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gfvvmcahj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gweecfixs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gswscdinp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gbzttqysi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gxdqpujzx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gtlnuuidk.sHtML


<!-- 参考信息 -->