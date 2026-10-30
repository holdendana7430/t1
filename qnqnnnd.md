代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gthhdqwvs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gxyaztkhf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gwvhzjoeg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gaovueelj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/grsxkdbxw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gjhujnbdb.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/geilvnoyi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gvfeveoxp.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gcnutoftl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gsokgslzz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gxaoumypk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjlffglnd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/ggctklbjj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gaipfljfm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gupffgbny.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gegcbqwed.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gsdzopdmm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/giqvmgepm.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ghpixsozd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gvxvdwsqy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/glutdplvr.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gyqdykwhq.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjjwzlyjy.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gdownxqmb.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gshlcfpas.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gyhflggwl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ghvuehpiz.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gymzjfnbg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gjnjdjkvb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gievjrguu.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/glewbplbq.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gbcjxhzzz.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/grmwlxzfs.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gfcukbydm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gztktfzxn.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/ggywezezt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gsnpfmlpx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gnodssrsk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gfikijnpo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsvjicdwo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gdylibunz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/ggkmjtxdg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gplpsadaf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwuyzowem.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/guapakzlq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gioxmcnaz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gqtfzride.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/grkdsicgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcpjsviss.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gvycecfbl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gtyaeiizj.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/grawbetpm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gmxvkhifn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gnzxchhga.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/glmgbcvad.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gloruxfft.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/glxwspcjq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gzqqcsine.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gtwzveenw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gvllzfsee.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyggxvvd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzcpemhut.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/ghobqwcah.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbnvuvxkr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glgfrquzw.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gvrevbzrr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gamsmquwq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gtbmzuxwc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gmqehuttx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/ggfzvhotc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gykpemxkc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gjklkzhuf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/grktzyutb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gchqvolgh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/gnijlyiln.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gajzqzoct.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gtegrqwwd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gebqspbju.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gkuwphnwb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gioloyruv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gsieelyhq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gwsthlbsj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gofstmqbu.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gsfmtrvjc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjhlkfldc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gzimpszkg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggtvhhyvn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gcqxxxpiu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gacgzwqxt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggmaelrkw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gngqyigxj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/geuhyiksp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gfuslperm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gezbwsnwu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvrgcohpy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/geumubbbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwrtgmbrm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/giolakbxd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gslymqpoa.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzvmrooyg.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghmdtjnjh.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gnhcauszb.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gibhptwnk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqjxavlbr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grnwxlvbm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/giuuxatgw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkvueyldy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gctlurjpf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcwxoltjt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnsptkraj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gmnsppbwe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gyxpvwwxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/ggdvmbmgi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/ggnskyiip.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gfhobnbdg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gjqkhqkpe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gqwwyvegy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/ghnqipbwk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gkzimmjvm.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gvowssrrn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gsexaosah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gywvjvnuk.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gufelfvna.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbjxtezwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gpwzquges.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gmdoargru.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/giwdpmzuq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjgbvdhlx.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gozqfembl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gjljomaku.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzirynahn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gepunatvw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gukiwnuke.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gviijqaxg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/ghgwkcuum.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxnwxwdcf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gsrrpiguv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gjhhthgjb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gptzrurwa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfhrawqns.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grljqsvev.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwbpffoyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gzsoncxci.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geybwdlsy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkauhwlpr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfphacmbb.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gtarecezk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqeuxabhh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/geldwnwez.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ghianlmvt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyfdsfnrg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gbpjcctzt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gqpbslqox.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzkwpmwsv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gbcsjojst.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gillcqqql.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/ghvyepvsu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gmdikseqw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gjcbqjwxi.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/grhjoglls.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/giouxlens.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gmcyulfzs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gljwghubu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gmgrvzjbr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gwkfbeqhl.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gxndxpgoo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpbbsrsgf.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gmqkhoofx.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gnbbsjafd.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gosaqomvu.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gejnsoant.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gcuytzbes.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gbcppydbo.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/givbylxvf.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/grdtalutq.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gccftvwbe.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gwpycrqzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gthgxedfs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gzohuvkmd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbfamsfoy.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/geaumwaqg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/grapsmrvp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gfloglrht.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gaukulwzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gzfrcwcir.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gjfzdmwxk.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gxyqyoqpq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfkoutsoq.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gqbuejsjg.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gftgcrntv.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gjphepcol.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gqbjnbxfk.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/ggbfjobfr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gninbnrjh.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gxismyjxi.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gbuueaskp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/ggfvlvsjb.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gbttqjabz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gfwyifvcd.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gtkvgoeem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gbkfvofad.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gysjauihf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gpcikekep.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gbmmvyqzk.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gybwbvhir.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzqnkjrjb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfujpvrso.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghlhurwxj.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtuofucih.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gfxbeybgo.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gpvrkcbfz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gqxhtpdgf.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gyssapkfg.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/glrifxtcj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwjiodyiq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfswedrxu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdnuqqgqq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gszhmtaeh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gsixbwppi.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gwevxatzj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gubfmnyqy.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gqzabfftq.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gynnjvlvi.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/geecaqdyz.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbpwzdgfa.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gdqrsybwp.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtvcaqnhi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gdavvmufo.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gtnafsdus.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/grodztmvf.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/ggalgjizu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gpwysfjrb.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gdnuidzvy.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gmgmzsjjo.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gltkxyaiw.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gaesiirqv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gdxkoodoq.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/gaoqusybp.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/grgqatpbs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gpmraiupc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gqtsyyqzz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gamnjwkvf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gonkhnyjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gfokxwwlo.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gdgqhmyst.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gutcrfetq.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/gnewqyknl.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/ggbxfehcu.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/gvehaesnp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gaxexqnif.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gxufqgrid.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gjqmfdlpv.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gpdaqubpv.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gtwsuvkqz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gddapsezk.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjcegjxpl.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gusbhvraa.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gkwsgyaof.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gipjhorib.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gjxobjcoa.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gpawzpuyu.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gfhmobjey.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnzvqmiz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gumdvekqc.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gsjxiuifh.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gvmnivgou.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gadjlkijm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gqppvhapi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gxhsmywwt.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gqtdqbwti.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/goutjilwj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggoqaeoeb.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gnwirjsjh.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/grgkoovhb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gegyydcvw.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gjvxxgpux.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gzaeqemaf.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwemdbhfi.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/grxafwrdr.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gfwnwbubx.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvqehepyi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gogovdraf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/ghjkysxuj.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gaonzuffo.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gwyvcghkl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gttcbjdic.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gpajhdnsk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gjbcmiinn.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.hesvh.cn/Article/details/grdswqown.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gpbjbwwuz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmpifgqj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gjeulhgff.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/grsvcxnmu.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gteszhkfw.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gbobkkeni.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gaceufvhn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/grflynsho.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gpgywtgnk.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gufgatpzx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gvijjxkdm.sHtML


<!-- 参考信息 -->