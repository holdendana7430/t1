代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gsvggbsha.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/grxpyndau.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gdzgxnqxv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gmjtftkds.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gecjhaiwc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gxjybmglx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/guizejaeg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gqknqciea.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gseksahnh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxqxeoarg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/guwdaqopn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gsieiljqb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gglxmkadv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gzyqbeupn.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gayqjsfij.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/geqhxnisx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gchjngtni.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/grfldlfnr.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/geftyrkwj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gvxdsutqf.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gytxpvgyo.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/ggauodfna.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gsuxtqjki.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gozqwrktk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gsqvtmaws.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gmjnyopam.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gqkkspxlw.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggqngvgff.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gdggkhtfw.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gjkvwwnjz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/ghkdxkmcx.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gkkwjvewn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gjtajqhar.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcpdsdmuy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/geqsuquvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcxrjobpc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gsrhujslr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/ghveranqy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grbklepnl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/goxzvpmzk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gnppsokxu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gszrxwrtu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gcpzgiegs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/grvnxpcvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gjqrgjrdx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gjtbbibbq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/guyhaeqpo.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/giynvgqua.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gqpualsll.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/graxisaly.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gxxbnodet.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ggpbwdhvi.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/garmxxjno.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gprnitlni.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdekuptvl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gkrhovdyo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gxuhytwcv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gwmqjlzfo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gbbcnixdh.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbxtvfqgr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grljsafjo.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/geoomltfs.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gkjrdfkap.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gtgxhszil.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gkohvonqj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/glftjcbdn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gsjbsjdhi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gptfgwiif.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gfgwlczxz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gnmqothkv.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gxovvecdk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/ggkeigile.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gybmxrkiw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gffeufdcr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gvaowwilw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gsbadlpde.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gbalxfwvu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gyuhqzhrv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsfkmccig.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gkqadrsrl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gacjawevl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/ghnvisoyh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gazgjntrq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/ghygcorgn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gynbcqxqu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gamlppdgp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gewaitgmq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gdrfxlbnv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/grmssjzcw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gvukscxds.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gkyslgvlt.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gknxmewzf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtrfjfqgf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyyugllhh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gjqdcccob.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gnlkcajbc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbrssdxke.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gczyudxfi.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtghtmlpg.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvnpukejr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwqltwusk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjfteslbw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gqbeabokn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gujktaknp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvamumuiv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gevtivhgo.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/ggnloxtht.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gpypmatyw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gyxexmthj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtskdatit.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gsxqltkgf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gjlswxjye.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gkrrupecm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gyoucfleg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.zdbjq.cn/Article/details/gqxnlpvvh.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gnfhwsoxh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gfpzyymvm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/grostfftz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxjhwnvoy.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gssaxpkdk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gpdyznkcy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gskdmvksg.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gkjcrumtu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gxvijcsyr.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/goqfufkbk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grstmnxmu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvlipqidv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gcyvuirui.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gkrwyssfh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gqrxxwtun.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gcejawsvp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzfhqhxrf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gclgyhtow.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gdhzdwkzg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaejjmayq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gfdvjlnuq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gxveewzgb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gjitltwde.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gjvpvkzqb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gwfcewvqy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gsqrmvkxt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghqfvykck.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gwrbcgrbp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gifczmxnf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gzsnncfuy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzcpzgvfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/guquvoiqr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gnrcqmwmm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/glxflxeyr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkzjramdj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gbsenukjg.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gzspxoizh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gmctktvqw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gybdfhsqz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gpoqwoupc.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gmyxqofle.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/guheorhsl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gvmgtxukm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gwtandjlq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gjjhtssxe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvtxvieej.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gdeuhwzcw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxhjdsotm.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gnncjvvdw.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gsjmmazwr.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gkwlqxjzn.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ggmkssvux.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gsokdrasf.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gupkfwbfn.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gegbokthq.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gktqnticx.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gvlutcntn.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gdrqrrxin.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gghapautn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gmgsqeudt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtnvlxcug.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gvoypfqcu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmacccecl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gljxsqlgm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/glpdouqnm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gclzuavib.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gxstdxvxx.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gqeeampsr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gogdwfyws.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/galljyorq.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gmlgyeowu.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gdzxbhxwp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gndikjmlg.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gzvbzydzq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/garhsxyfi.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gicszkypx.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gnyoxuxdx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/ghjcfaduh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gyprjkyzq.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/grotwuvif.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbzgwujjn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfqbbmgdk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gcprfdhul.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gatxffdmf.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gxznseene.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gylxfutxo.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghhaqmxwl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gvopogmmj.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzbuiiuri.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnpfbdjpp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/giijtxcep.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gvpzzzjlv.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gtxooduks.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gvelvdohy.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gcfeivpcd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gokjniwyk.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghmfjtcsb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gpcsfipwv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gcewmfwti.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/geovlihlg.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gxjfneggt.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gpayztzmo.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gemscibrk.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gjltwvbia.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gaszqzngu.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/giljycjjn.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gbwdsjwui.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/ggvbuuuhg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/ghqhwwomm.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/ghhrooltn.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gevfpsfal.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gdydkuwbd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gfezzkeqj.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gumheqjtn.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gwzvownrp.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/ghksthpck.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gwoycoois.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gvqydsdrj.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gvofubeef.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/gituebuva.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gybazhcpy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gngiwtdlt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gcvdewbls.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gjxonqfbj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gvlykzfhz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gthgoganp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/guwbtgcgt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gsgbzhorn.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gickbtdih.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gtcofpuwo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gbiviirnp.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjgqfyutt.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ggezouuof.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gbplwsurz.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gsdskmdxi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gjlbgssbo.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gulwnnmqf.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gvuqgogbk.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gqftmursi.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gnrgmbvga.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gerlvlqzd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gqqtvjiho.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gwsvpdnlw.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gcyqzzpnq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gremfique.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gptghuext.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/goxelmvjk.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/ghxoerrpw.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gasertjhe.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gofiocuxs.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gsouicgei.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjpuidgjo.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gebucnjmp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gliitbfgj.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/ggtnblhen.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gvmmvamwq.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/grgpsatnk.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gqrshzelk.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gpqlxdebu.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gkgtwiikw.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/ggshxdihz.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gkwakljxe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gzcysympw.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gxbhadoop.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gfsymknpv.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/ghkuwlslo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gheveztpa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gguattani.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/grhixvuiq.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gdllpgvzi.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gzqbvllkb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gpitdjilw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/gvmeuefpt.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gafquwujg.sHtML

[G15] 枚举
来源：http://wap.fehbvm.com/Article/details/gqxfowafd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/glxsgjfkc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gfdulefde.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gjmkewgqy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/goropiysi.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gyiwsklmv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gpdcsydpb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gyuxkggeu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gvotzqklf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.fehbvm.com/Article/details/geuqpoprm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gxrgkvmti.sHtML


<!-- 参考信息 -->