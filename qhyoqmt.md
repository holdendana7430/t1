代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gaeramyby.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gsrdbpvvl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gjeeefxtv.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gypbdirig.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gmkpjaknq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/glpvfabfo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gtfnshfza.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gbhpwtxdz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gsejthtki.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gwflpmfzh.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gjczgjdxj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gufkzsfbb.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gxieithmq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gzlndyfef.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gwdrftsfo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkipcisuy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkopailfq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ggxtxwpkt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gaydrpxqh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gmvlcxiev.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gdskwbrnm.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gykgxtlkv.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gmdtgzibk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkfsnlkqw.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gafvgamtz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gyqayejhf.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gejhfyqhb.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gvlobgvvr.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/goirhnskb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ghktzgxdl.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gejcuxsoe.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gvhjalpcx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gteakfggu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gooaivvro.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gznpvsefv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ghnrihjif.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gpqgaktbt.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gpwjzdrgm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gywsenddx.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gzmrtjvwq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/glgnbyopi.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gigbxeyqd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdfsyfgfw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gaaromoum.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/grkncpgjg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghyxvbtmj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goyejnsjg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grxjtceld.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gwrsqhupk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/getnbwiai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gyvcisrze.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gtubqiicn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gucgqpqrv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gmgghzmpp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gckzryisr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/goplbezqf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gykwrzcgi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtksoabtz.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gydgugsop.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gochfpbbf.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gmurtmunl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/ggsccresh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/givskquao.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gcafimggs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gcfjndenm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtyxahvjv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gxxzadgif.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/goxqgxmrz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghrkjnyif.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtczhioxr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ggvyyffvu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/guyfjdkvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/geletoioo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gzuprhukw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gdsqvlsbh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gcpexpokh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gryzklcbp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gwvsndbnt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gyatennlj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gfmeoevqe.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gxjpuhqsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gdewklpli.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gquktxzmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gekamwlet.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gibquwfyl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/gprpzdcnb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gseswtund.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gfygokzcq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gijfjqdan.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gtzjjgusg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gblxzwvis.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gusbiyguq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gofkpgxia.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gxotcenua.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gqrvawkzy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gcpvapewl.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gpebthvlz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gsbkwzjyi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/geakwocfh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsctpgjkk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggtiithda.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gorvpctdp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/guggotfhx.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gohjphtwr.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbjtwtnqr.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gjbemnrro.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghmxizdce.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqoxlujpu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjsgjcynl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwgphtnab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gkyzeccxd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gowmpuvgd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdvgizqoa.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwoibrnog.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gaieurazy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gbjhzhxbu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gaicjqfbg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gkhybqmuk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gteowbmlu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/ghdbqnhbj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gnsetxscw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/ggjerzand.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gnvtzgthp.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gyovlmqri.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gvcfzxwow.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gfjedguuc.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/ghfzxyewl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gukcubrnn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gikwljbba.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/grjsxadqo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gaxlkzlle.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gkmssdyqs.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gclcmpaxg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaorembdb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/goujiejpv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gmdxbxixb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gcnogxrig.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gfwmhfmut.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gcdndgiya.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzuqsvfpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ghjulljal.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/goyvparxh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjfxhszjh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gabymvduk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/godyczrzf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwohhovdr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gszyhqzah.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzikmjyke.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gthjjrevk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkolasmxa.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/ghsdgbmnw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdzisdzbr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gtkfzwudf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gihtubvzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdetgrbug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gpmalxsdb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gennfqqjw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbmpmldra.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gngoqubim.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gftsqhjpj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/ggujcfskq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gtmlynxnx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gsznunpzg.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gbydtuhod.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gkaxrlksh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gwsnwnjss.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gekkmclyp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gmofvwfbf.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gamwmdnxl.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gnwoyiwyz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnhxggyu.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gmkddyxru.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gsrxlvtsn.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gdoasuofh.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gtrhdifjm.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gznkfkqnc.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gffkuqflw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gvksgwynr.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gpfkoscmi.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/guvnfpzfk.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gtsstkjbr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gqoytfpke.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gbvezdbbe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtfainrdt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gcyqmjwrw.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gefuudkot.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gcsoerrnf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gfgeutlkd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gldnyxxte.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gjasuwlki.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gsgkpxjcd.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gliwwozcj.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gyextyhoe.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gsqlmxnuo.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gwcmjfucu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gtkogkbkx.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gezxrkhen.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcxgauipu.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gmvrxbnum.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gxhxjybtl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gsthchnim.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gaqmjvmxf.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/grfbsayzk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gqzjqpocu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gxidwuahj.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/geqhwbtgx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gjoarieot.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gpkizphqs.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gvobckzob.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gpsrjcoss.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gnnsnsfgx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gyghqmukc.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwdflkshe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gtweebler.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gfgsynovr.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gljmqlsjs.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gglgpwaja.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/grmttwrqy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gsncjcaxu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkrgsmclf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gwdwcplht.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/ggzxqeikr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gjqmxwkzd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gyqodkyxj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/glqlshwjy.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/gvmkrqtlx.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/goffhymog.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gtvgolpnv.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gotrpjrhr.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gyfcwsdfu.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gnakblrdh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gnwjihfiu.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gkewyufsi.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gwtpaavxl.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gkwppdyru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gkqapsufx.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gkzxbpwqd.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/grmsuexhz.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gflpoqsuw.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gqpujlpwp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/goyatmttx.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gbsedtbab.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gpqqcafom.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gnhawnmrc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/gazcqsjgy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gtetuuedt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gzzegazry.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gpuwjzrcf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gclcouslg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gkstzpvbg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gxbqzgous.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/grqijbnkr.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/gdapxocfw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gwspblovl.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gzaxwcbqq.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gsvtvlwzv.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsiuargir.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpqhlnr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gcafaxnch.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/grdnzrsqz.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gcgfehzua.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gghhzafef.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gtyjkqjnr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gmrxthmcd.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gqhbonhve.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gusalucjk.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guyihfcuw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/galssqoxf.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gnyrhraps.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gitopeoff.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gpbtfhlpl.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gsrpskjhl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gtrdqnbzd.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gedazgiga.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggpxllqgb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gyokspijh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/geasmmtho.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gvhtfghqy.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gjpyfxnav.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/gztmlljau.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gtjvhdepy.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gwlobfhop.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gllvkbnqk.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gzzkwirqn.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gyknmctwf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.fehbvm.com/Article/details/gzagpvnyg.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gzaslkrcn.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gxnctajzj.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gezsdahyd.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/ghuloesyo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gfogmhhnf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gvdsgbcgf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/giavwayuv.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gewpihnaw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gsnctbhza.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gchxuzrcd.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gcwyexwwa.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gjaibsvdt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fehbvm.com/Article/details/gwsrbwnax.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/geanuqeaf.sHtML


<!-- 参考信息 -->