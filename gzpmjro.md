代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gtczneupb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gamovnoow.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gklbjgvrz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gkndpkdgb.sHtML

[E18] 模板占位符替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gencopyxz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknifzliu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gfcsdahad.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpepgmguw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gfldvjmrv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/ghzgidtws.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxcltumk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gidnfgnot.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzizhoedj.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/ghcfbhnkr.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbztegzlb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpzlqhgu.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptzkdml.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhaudxbp.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/geclnkjyx.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gskdmuish.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvnbxeop.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/glibmnawg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gdwsbrkzr.sHtML

Py:   if not s:
来源：http://blog.fanxiaobao.xyz/Article/details/gzwtnonmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fanxiaobao.xyz/Article/details/grrcfqhwd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/genpmiism.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/glhbkrfew.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggtzboydo.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggvbyjlgg.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqfyudqu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/goefjwleu.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxipulznu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiznlgtt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvkqcigh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gkjtzqtoq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrlrrizs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gosvalioc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/gethwltdj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrwhfojz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gxcpqvsgq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnrulrivh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gynglelhf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezecozwh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gkqwfkiut.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwauayixn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrdniskv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbocapnmx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcikgdzr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gklztdqlz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzuamvhq.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwitjcnsa.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcarxcsr.sHtML

[F01] 读取整个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbbjumfy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/goxvfjuvz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwlzklgh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwqzkiwj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmpvbhw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzhuannw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/geqvdhgzv.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gofmjtcbo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gonmjfutz.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gsqzpzbyc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gaipewxxx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gptehymli.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwxwkzua.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gmxfwsccm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxprmgqu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/gnkfjqrjf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/gsoqmjrnj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkidxzc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gnveydanb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gtyfmnqoa.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaotsbtk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gptzihohe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbrkunrp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gsimrrtqw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/gohbmcxqf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuthdfnw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsrhbenp.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkwhekvum.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsvlmnlz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/gulscbdwr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gktutumts.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gkwnhisub.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmprhats.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gcpjlptfm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjlveduk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbhqojhs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gujgavmyp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fanxiaobao.xyz/Article/details/gfhlsahxc.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gblvdtngp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrayixbl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqzaoqqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/grfjefjhb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fanxiaobao.xyz/Article/details/gneupeoki.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvwcujr.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvhppvoh.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdplyzlgl.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcyyzmghp.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoqztwow.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gheeiliub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gxrrrnpea.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbixocg.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzsrxsqa.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkfgqiiyd.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gncnnznlg.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwnpenhq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/galwulgxw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gthrcdycu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gbjrfrlvf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdscypih.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gugctnizh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpupgfxwc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gpastnpin.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghasnppdg.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzemfjnqc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbxkuieh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsgzpjdoe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbjomcrn.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjrenkxg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtayladv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/grtorxsku.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gpsapodjl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhsdfxtm.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxykyhmw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgtwerll.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjdvtbpx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/ggndroewj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gwvyqvuee.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gvldjwlws.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gchaxxvpx.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gvxvodtkc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukzofopc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gyhcqojop.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gusalfntr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/godmrrudp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gplstyuyr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/glaitqhlf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfavnexy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuiinqay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmxblcpj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqutiebl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzecdsjn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbchsehga.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gpfinuwza.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gupgxowgf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbczmevrf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkymkybmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyfjmofy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gqcwxbzki.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gikogodwi.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gorqldzit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gxdevuabk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fanxiaobao.xyz/Article/details/grghfhnpf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzzsiged.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gsxespjhj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gkdolhqfq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwidgvko.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gniqwqaap.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonduezbg.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gubckmggr.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gslcsazkl.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gmhuygnmt.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcygyjaqs.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjtuvjwg.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfdeqmgf.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grtoxxvpz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdjdropk.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgdiuset.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gadgzctsy.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gjeijfrwh.sHtML

C#:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmxzgryw.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/glokrqnss.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fanxiaobao.xyz/Article/details/ganglobde.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcrbyjgj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvhkttbx.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhxjpyve.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqgpqalcx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzqwpayjr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gydetksij.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gizwbjmlz.sHtML

[G03] 实例属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqazwvfu.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdscikuow.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gtzvgsjmm.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkkktcqr.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwvqbarl.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gazpppiih.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/goggitagz.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkybkuxz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gwweeqkob.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcpshdmw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxragvqr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gysfzisak.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gewixjxjo.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgrmtgbl.sHtML

Java: String greet() { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnizbcqz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxsudpdc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotyckxfn.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaaoknad.sHtML

[G05] 继承
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafpxksn.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gleoujllc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/grlulfkar.sHtML

JS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwtrwtwyh.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxiwzyidc.sHtML

Java: class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glzhqimpw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gygftlvon.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeyllvtt.sHtML

C#:   class Admin : User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmuwyegfk.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gohoooyxk.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fanxiaobao.xyz/Article/details/gxqqeidmd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvfogvfb.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/glwexekcm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gumnsqxgr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grccajihh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrnjwpod.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gtyfgnrbh.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gzrrwssqb.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gnbsrkuml.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gdwxaaiwz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjahlfeid.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gtmtdadcm.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaovnvjr.sHtML

Java: super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gknymznmo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/gwffibgtd.sHtML

Ruby: super
来源：http://www.share.fanxiaobao.xyz/Article/details/gzpbfpfgq.sHtML

C#:   base.Greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gsohruaew.sHtML

[G08] 静态方法与属性
来源：http://www.share.fanxiaobao.xyz/Article/details/ganowhlnl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdducfuj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzklmskkv.sHtML

JS:   static f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gsscuaxao.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gepyekgje.sHtML

Java: static void f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gomfjlchy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gegsaimmo.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/grbpixssn.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gvxwappvb.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fanxiaobao.xyz/Article/details/gvbaixcuh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhrheoup.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fanxiaobao.xyz/Article/details/gipespwsx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjossbkez.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghcvwrdlv.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtmfmtudd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukuskyob.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwfmrqow.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbekbzwq.sHtML

[G10] 访问控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdfmhyge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpyeskvc.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/goiyyzjvp.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyvhrsoc.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxlageez.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fanxiaobao.xyz/Article/details/geadwcbef.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/ggvdsavla.sHtML

Ruby: public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gfhyojtrv.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gezlhsvih.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjldazvb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fanxiaobao.xyz/Article/details/gimtdtzjt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gixihucvk.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqrlbqfy.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexsjfohu.sHtML

Java: public String getName() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gaeckofge.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginywpycc.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gwvtahlna.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqouizbc.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghjungtaj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/giosgvivx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gctqoxwwn.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtjbxipq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdtndirbh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/growcyqlp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkkwmoltt.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gndtutadh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirmjqav.sHtML

[G13] 判断对象类型
来源：http://3g.fanxiaobao.xyz/Article/details/gqjzwxcrq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrfdody.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmvjenzb.sHtML

JS:   u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrkowhie.sHtML

TS:   u instanceof User
来源：http://3g.fanxiaobao.xyz/Article/details/gambioltc.sHtML

Java: u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/gibgtmgfs.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gpojbvwjn.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxupzbqjd.sHtML

C#:   u is User
来源：http://baike.fanxiaobao.xyz/Article/details/gthkrbklu.sHtML

[G14] 数据类 / record
来源：http://blog.fanxiaobao.xyz/Article/details/grdgyxujj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fanxiaobao.xyz/Article/details/giyyeaicj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fanxiaobao.xyz/Article/details/gncjafizh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoywzoyu.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fanxiaobao.xyz/Article/details/gasnabibj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gasyghiyw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fanxiaobao.xyz/Article/details/gtuczbiyk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fanxiaobao.xyz/Article/details/goegosiih.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqbcpwul.sHtML

[G15] 枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaleozer.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gijfabvjc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbfhxres.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvqvummr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gaufngzuf.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fanxiaobao.xyz/Article/details/gmvkigwpa.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fanxiaobao.xyz/Article/details/ggzvgznxt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsezqztg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsldullht.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fanxiaobao.xyz/Article/details/ggezvczgv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnoepvzji.sHtML


<!-- 参考信息 -->