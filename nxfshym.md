代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gactcxnyk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gnwwkvxip.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gowgvkphe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsdshcwj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gteykbdbl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gjnyjhjnm.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gdyclwtqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gkonbsyfo.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gpzfvjvvz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gxrpjnyve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gdfuxnmps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gaxuzdaup.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gcdkyslyd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjqmrctoa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcgbcqwrg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gpycwhzpw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/givxolkog.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gmtiryrps.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gbizsvfhm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/ganvkkxaq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gbyowwkpw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gykzebjas.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gdnfhyyhf.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/grknkkmta.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/grfrrtqoc.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gjetpldzc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gaoxtyfri.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/ghrlzzhgh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/glieiglha.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gtkcpvckx.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/glqrsyjze.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpdkdsgcs.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gtthahzgt.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gwtvaayng.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gsriybytg.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gyzchecze.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gjlubuegl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gphmmxize.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gwsfkkfie.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/grftrqdoc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwuuaeqcs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gywvjbmuw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpcjlcwmq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gkjgmyset.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gjacucrce.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gylgxyjbi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gjihlrqcw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/godxfebwl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkzeycjly.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gbrbvndwj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gqfeqldki.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/ghjycnomt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gzzpdkvzl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghayugzwq.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gylndafhn.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gamulzvvb.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gmnoibgjq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gcpefzcdx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gttuqsfxw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/guiuhvpnu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gzfcffxvo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpgrijrbb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gyjgwurci.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpkeyhyhq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gyvyefazc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/giwyqydxo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gvptyyozg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gwpayshdj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gyjwiresv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gvctaxmpa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gmmzkxgql.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/glggndoke.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gtxlworav.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gilwcgsrv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/grmadakyk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gubwtogeq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gklchxgar.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gxbmqykqt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gttlrmnjm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gfcivavkm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/goraapkrt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/geesfymax.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gypkvdxmj.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gashauxhm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gfbdhunvo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gzrfsihpp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/glvkyxrtm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gynpmdiae.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gdtqrauwz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gudctccww.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/ggrwxswmr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gdczomjoj.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/giqlrdgqk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gbqmbdijt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjninymdf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggpngwvjj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpjkmtlwo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gitbpcggr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gczdrplyh.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxzstkpcu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbwafmkyj.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gttdwfcss.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glnveobnl.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbtxswhlv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goztwhhbq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glmxjlvkj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gpeeekguw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsiuwfhrt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gqmdidujl.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnujzpkjb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gpdalynlc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gckbzrcaj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gpxzjvsph.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gtqgzkung.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gzpfdxrfi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/glwjubvid.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/giuptbgsa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gsvunohin.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gygmecvwh.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gfflyrtxk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gujbrypix.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gkesyrzhx.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gqqdvewsn.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ggijtjnxl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gftjbutkb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gsgfaeasf.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/gtyrjmlem.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gvtrcfjqr.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gznhgvlwo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpbzmmfav.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gdrjrbxrw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghrictslm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gbczjjbkp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gtkypnimz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gmgzvwale.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gafqafqcl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gpoviofrh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gcyvwmfiz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/geurcenxe.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guurftjfn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmpstpajr.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggjkowadq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/geelpaoad.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gytebsunm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbktyylzw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geuqhwlav.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/ghyryooig.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdseijgxq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkyzrvdyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/ggliyauud.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gowefzjta.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gxidpfzlg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gnqhkejvq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gldqvyojl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gimlyiuwz.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/ghkmbbcir.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gmkjfawiq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gzdjaciaz.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gypjqkrif.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gzksmuuzh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/ghhkryneo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gpptmrdgt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gulmxaudx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gnybxoiwk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/grxfcjntp.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gdzswxkva.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkvonswrx.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gbnpvyuwh.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gnedibpqf.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdysjabfn.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gciskjlgu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/grtqijqzc.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtvyolxcw.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gcnbcuond.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/glsxnxmpt.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ghshecajg.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gmbeyukvh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gazbwrtmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gvkwtvnbu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gumvixuxq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gzqqldycu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/grjcklfkh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gfjmunksq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gpcuwvelc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggjrxvrjy.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/guapleukv.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gseoewivk.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/ghcdkbxmv.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdnwbzq.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gylguwkkq.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gpqrnxsui.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gyzzeerqf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gzbouclmy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpcteajek.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gdsmqsfaa.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdjoynrts.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gotvunawx.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdnxchpgq.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyhjmqzbp.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjwqvpzph.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gzaclcuig.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gjxayltsw.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gyrzunmnv.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gepxntpvc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gjvdrmbtx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/goiuyyhtp.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkcbekirb.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqszpwlfr.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbjwbjfhr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gutkuzvkq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gangbehte.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/glitovjdy.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gfhyssjmm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gkmfmjjht.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpxlsztyf.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gglgofock.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gqpqmlpxy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gexljkbtv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/giraywpxd.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gaottwyul.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gxnmviiux.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gyapueluk.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gpbcsdvbe.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gflcwugho.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxmabrveg.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gctigjbgf.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grrzbbxlw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gemadnewr.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/ghhidjtht.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gvauqnwhq.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gjaxjrzaa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gvgdkmyck.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/goyxxvfct.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gczjhlqbq.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gcruhsvhw.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gsnjawbjn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gsvboxddx.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/ghprulihf.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/geatppied.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gujmpzlje.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/griowwwmv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gdumyhgum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gndxghhfg.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gbcyaztiv.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gdqsrwfvk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gcdxlqidx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gdibizdqz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gzqlnslff.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ghxujsbop.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gmenppqoq.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gxfbhmrgb.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/gjwhmsvqn.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gapskeqoc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/ggobwoboc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/guobrnotz.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gurbikfzd.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gmriiqmnd.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gujaxhbfe.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gasazmwxk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqnaxguqb.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpoqxmxvm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gxnemdjtq.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/grksynpdg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/grhyjmkkk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gkbwxslec.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/ghmokfumn.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gazezckti.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gsfjdfhra.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxihcxrdi.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdqzkhjam.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gmqmorejw.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gwovdistr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gkchefefy.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gdomeykug.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gqolsrlca.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gfdawwdgp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gzgynlane.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkjgvhfja.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gwflylccy.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbrzvqbih.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gsldsnfuk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gakqcntju.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/ggnonvfyz.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gdcsvdzjo.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gnwipnrnz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gixltmwbu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gnoefzcjm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gplkipqng.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gbxucnpkd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gktvaqgdq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gyzyfgjzw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gyxvmzhfr.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/gyswadjpj.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gwknaghhy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gjcyapkke.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gxtnbldui.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gbxboxdyb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gugestbxg.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gopmlposw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gbhzizdrw.sHtML


<!-- 参考信息 -->