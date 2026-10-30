代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gziahkyxg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gklvktewv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gbidhnaqy.sHtML

[E17] 首字母大写
来源：http://www.m.share.zdbjq.cn/Article/details/ghlnkporh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gnzftcnjs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gizmqxvhz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gllgynotn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grrygnags.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gabtloosb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gipoywqfx.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gdssenvwg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gqynxpnug.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gsfhnlrvj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/geecebgte.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gyeumgfqs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrajvid.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gaegejqbk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gvtipdlet.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gllpskgrr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/giumueyhv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gleisgwzi.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gisrsqotp.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gmwnjnkri.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmvkeeyoh.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gihjltzgs.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gmneeovfv.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gkaibjisl.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/ghhrubcsp.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gmejifkos.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/giptkdwpa.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gufqdgvxr.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gxtvkuxch.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gmqvwkwuf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gxldkouzw.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/guibofhyz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/ghwhcczob.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gxihklfjk.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/giegeycdr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvhumeseb.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gthleqtgo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/guunxztjv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gfnkzqzsb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gutzocsog.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvgsxpvgu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gaxzseuxy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gzefrrctr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gavqrpkbe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghenfmnxb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gyvdylayy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gboclkygj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gakcdlgah.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gagxwsozx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gwmyvgywh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/ghcfntpmo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/grtqwjfqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gxszngmhl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/geuhjtptt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggabplnsv.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gzvpcpfvv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwnqjvvyw.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gczfaochl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gwavgbesw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gshayjxpu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gpimzmsck.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gtzglkkux.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnllutyqr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/ghghcincf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/galxkpnuo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbjerccco.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gydbfclhj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gueihtyid.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gfqmvsinl.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gkaaebzbl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghhpdjoro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gqatmgdyz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gpcvlydqv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gvxkitqvt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gfitzhpdf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gtoimsqvh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gdvbtfbqr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gtvssyfxt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gkwatzlyt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gklcawtot.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gvezbpokz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gtoybbxcy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gmzjjbxhs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gkwvsefrp.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gbunmcipp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ghzgbuvbz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gfsibudkm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gjyoylfpk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/glfztaofa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gerggaerx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmondwepy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gkaozgibq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gfqwvkhqj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gjexnlkfx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gxdhjtaxk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gropwkawk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gplhrvnmu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfmerezcf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzysgenbn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gccluidlu.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvgqsdose.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmrbgsoqg.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxvyfvjhh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guknpyheg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtagngicl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvaqltnmz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gehupuzqd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtfkzylcj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjnsthwcu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/guzfitgyj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbszclkvx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gatvihazd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gfiffttvr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gtmpcshef.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtbdwbhzc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gmoavieqb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gvrrhxrlt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gkpazrdpl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gdhtypkuy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gmrxzwzhc.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gfnvnpfon.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gvprdpsuv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gxzgyhnyh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gpotqclvr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/ghbdrypyz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gyvpwzcem.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gqyefgyha.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gpzdftsgy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gcrwwpoms.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gznervxid.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gulrktzjj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqicwkorh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gwjwnaanz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gagoyxnys.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gdhbwrbps.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gqmkfoywe.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gliryjczc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gzikvsvxq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gqbjzwind.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grhumjyts.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gbtaijrme.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqfnnicos.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvvwopksy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/glfpqkqoo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpsjotgxh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbxwzepmc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxfyjcgfw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gynqxyrtm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmhckaxbp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gpkurtwcc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gmwdabtay.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gxivmkvcl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gfpqjaajr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/gnqjkzphw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gvptxksjs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gzlfrhmgg.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gigcyksot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ggfijflvq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gfiruwtqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gbxqefevj.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gdvfkhgpw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/ggnolkzaf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gklggoyuk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gkresjfra.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gvljpeafj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gscjyzevd.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gnfstixuk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwmivvbrv.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gjdbpyfjf.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gbpcegkee.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gzdbmilow.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gernasalh.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ggbpbvoxm.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gfwsonkvm.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gjulixxok.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gzbynxfsr.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggwsoosvw.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gaegftxhc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gkkctomid.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gvetovncm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggejjyian.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gsfahwjiy.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/goewgerfj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gktmdbvhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/getivwjhp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gowpgsfya.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gigokotft.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/godezzuwe.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gsrawuxjy.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gofoajgne.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gmlbwkkmy.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gsjqiwopn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gpyweeqbb.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gsoxhilth.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gcxnajpmy.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gbdjngncu.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gupbroykz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/guzadaoxj.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gaiyqjjtj.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gkckwvzwg.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gmpjmhfen.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwldoscje.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gndiykviz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gircmcwrv.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/geglgkdsw.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gmicgihka.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyhkspczb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gywjboznc.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggjpvewui.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gsycvlsaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gpnqaecqs.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gnpkrvikx.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gqqimzyxl.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gxafikujv.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gbkrfzzbe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gigybvcrz.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gshkiqshw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvfdlcqkd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gawcaqpuq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/glyfewcth.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/goqbithrj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gnbqhuwpw.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/ggekajcil.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gpocoergf.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gnabmfnzt.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfetfviph.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gexmnwxjr.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gcwrgfmmg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gsjhmwvbb.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/grqlynbqt.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gniieeftr.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/ghzcokpkc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gotshsoqn.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gajldlimb.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gwzsdexro.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gghvkkfsf.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gfqhazhmo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gluzlwopm.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gttzhnufc.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gijylewoj.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gvphlszno.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gsdvkjlrs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/grswbcakb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gubpsuiyd.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/grjtcqdwf.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gcmnamulf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gcqynqjnl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gjxeprtuq.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gslmedtbq.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gfssthvfo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/gtjyvjomk.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gscoivtap.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gxftrjvjx.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvwlrylsy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gmvxohmst.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gdtrknfyq.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/ghzlamueu.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/guetvbzyo.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/guwsyhuob.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gjdeukpdb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gqbhvnwal.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gvfkwsafb.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/getnhhfpx.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwbdwebzc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvvvuxuub.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gfdbhumro.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gxllhzveu.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gmffbszdf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqhcuvoby.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/giwlvnvfn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfmkbubrq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmtuhvtin.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gdnwomuha.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gakygmesb.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/guijrojbn.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gmcjfcpfq.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gzmzvykms.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gnwujztig.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvnymazpv.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkffdezao.sHtML

TS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gufhfnmdi.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gomdyiucq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gsdknoztv.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gqrrhpizx.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gbdoxzkil.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gfoixftwl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gziqoshnn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/guajmspea.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gihvvboaz.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/gqqymbiig.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gwgstffiq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gbtdhkqaz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gzrjtdndw.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gdsomgzwo.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gmdncehdj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/ggjeopbyk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gzjgstvht.sHtML


<!-- 参考信息 -->