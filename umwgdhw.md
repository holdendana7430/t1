代发 wailian999

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gzbkzqbpj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gmjsnndgc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gwpynyjdj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpfzoyazl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/ghbxbfvqp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gmeeqvtjg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gtvuepwga.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gdiazhulz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gvylfrzmv.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gsbrpwbiv.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gxuuyehyo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdutqbjbw.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gbbuepmwl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfqhsivi.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gywnqduaw.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gavwyocuj.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/grgzwzkbw.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gtqfoomai.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gsizxzcqh.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gduyiqpxn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gnyppwuoi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ggodfhang.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/grzamdvwp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/guvgszxbv.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gkekltmxx.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gyqhsbpcr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/geybcwuck.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gdnieemig.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gqcdmvrtd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gzdyoeeci.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqmogwkdb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghezvxllv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grbyeigei.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/ghgykhwcm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gppuiiaxe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gzlchodvq.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gkalqogil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gcbkpgdit.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gciggxakx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/ggjsfkrqd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gfjrwddti.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gczokdzhz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwyrmnnoz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/geapezjqn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/ggsrnkgyt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfclvjinl.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gdzfrerod.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcusadzmk.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gflcxatvs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/grgezqdzk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gbzebnjhj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gzkddxhww.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gcjafqqgz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/guqnphwzl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gcvaepmbs.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbnmbzwvy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxubikhqy.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gqsqrduul.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/ghrerlacu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gbwvdjcdi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gpdwdpply.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gmpolzkca.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gnbpxneou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/grqijvwzt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gorcacefm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/golewplwd.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gttgudkfo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/ggkfenmug.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gjlvwkypi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/grhoppjwq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gtjmdnrpx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gnbbexsqd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/guyvkouiw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gliawsccy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gnanrnhwe.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gjfikljzw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gynhoaakr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gdzknwtgr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gloczfkle.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gbfurhjef.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/ghtpjwkvv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gixheenbo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gqyhqyszc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gjjqgylpz.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/ghblrwqwy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gcnlqqvul.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyycjeahx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geuixhpjr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqmfeuxrk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtcbejmvo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gffuyimgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjmsryfwn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guxpedrpr.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gmytubpxv.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjbwuwqr.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gweyoaobv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcnmesdfn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmdensjpq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtlcjhpwu.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gchiuakun.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gonllgxri.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbmdcjfgr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gieqwhezj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/grjsnfeir.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/grvqfrvmr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gbzavsace.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gckpnbfir.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gichzftts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gqqbmwpkj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gngglvpzu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gxgvhsiwf.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/geaimufkt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gudnefuyx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/gdgrtybqr.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdiwgefok.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gcmxykaww.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gyfvlfzeb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gfbvfqwph.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/glcokkows.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gpbrdzkim.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/ggfzmvwxe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goqqtgkdi.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcwxxmkmz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gtunwuikb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gqqqdnrdt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gsatjixjm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gktckqjxo.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gibeptdsz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/guhogvesv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gwwtnnreh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gitzhyffn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/geoaranjl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkulwlwqp.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvrhddpxf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gmumxkfxh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzpyabthc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvqzqkhmq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpcffiohf.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gmzsnjwta.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghqbkqgbc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gthbhdjkd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/govxohftw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gruqrgxgn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gehemvmyh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/glhubfjdu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gtqyaofec.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gmxvofmqb.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gydgaydcx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gclqkmkkl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnsdvpk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gygvfdopw.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gfmrdmtpp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gduzxmnac.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/goefxnucx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gcgueytqg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gdlyjrvan.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsxrbjmmi.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gsbtzlzkf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gefabzbdz.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gyxgpcfdb.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/ghilwwkoh.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gfbpqxivy.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gfteclwzw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gwteizqyu.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gcpvddull.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gmqlzwrne.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gwjktyrtl.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gokzdqept.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gfmxiegbo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/grusjhwdv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/ggvssywmu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gksodkmlb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gkiecbvop.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gdwdyzfgg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gywplayef.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gtqjcspfc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gcavyxcvy.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gnfhutvnq.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gcducdklx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gflxuszba.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gztxzorhd.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gipgcbgbd.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gdybuwqbb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gqtdwulzt.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gqnuibjmc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/glwlbvgcf.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gijsdojid.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggsgtgwoc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gdlbdtjak.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gkwujxnxv.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gowpgvsos.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gmlsdaqhu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gcllaouts.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gkhytsbvl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gvdvnyjkz.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gaawzqbng.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gstcbuzlt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/govxyqtfi.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmpctgkah.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/geebciwco.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnomdvpdm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gjxoxnkjl.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gzmoqzquo.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gyjhqwjmj.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gbvvcjwhp.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gmqwcqmzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtbodtkdb.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcxxbldne.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grvaeemcx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gbyytijgl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gkyhjytnd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gsfzxyfrg.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gaprbrisj.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/ggqybpfkx.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gcydxhwsq.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxgqxlhve.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gphmxmacv.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghnypbhuy.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/glhmhdhmp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gzzkzltyu.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/ggceawymx.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmcuoofgp.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/ghuyxvugk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gwbjiknuf.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gadslruzh.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gurqapzkg.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gxbdhndjk.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gpivaddpj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gdimlvsyd.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gaegenthl.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/glibgiedb.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gueeypiat.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gpnszomnm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gesiomqvd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gjtnylpss.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gfyrupxjj.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggtcuyqam.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gqjrjfckg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gcncxxiaz.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gwokexwhf.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/goflmduky.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/goisjfpbn.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gydyscoie.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gjexyfhsl.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/graiwavho.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gsolfqnrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gfeprxzyq.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gagaeyqne.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gtbvxccry.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/guxyapwvu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gwtzqbfrr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glrwvbxww.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqjabwmny.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gwuxjxoce.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhrexzte.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gtecjfneb.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/gnrvxzljx.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gqmbpfrxs.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gtssvuujx.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guivzncuk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gjrnotjjw.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzqotiarl.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/grubabjgd.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gizdheasm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gwscsaztq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gvngmflef.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/giwhtsebr.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gqgqzyhus.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gjvubnszb.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gonvmkftr.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqukitzzv.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gvkngjpcj.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwjtkxybm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.zdbjq.cn/Article/details/gqvsdkmie.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gfregakxm.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gzpholnjd.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/glxhdnicx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gdleoajrk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gnalapwjc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gdwtuvuft.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/ghbygcjoa.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gymrlvtdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/glydbkwwm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gaamxpxnk.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gdtgmvhhm.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gtzfqczfp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gazvjwjfy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gwboirwwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gztptpiem.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/grzompkbz.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gwzccpdbu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gpgcvwgro.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gphmmdiab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gmjsrvlbx.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gforbsnzb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/glglfxbbl.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gaaiihiub.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gjlekwqoh.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gnpviwmnk.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gfsokhfsa.sHtML


<!-- 参考信息 -->