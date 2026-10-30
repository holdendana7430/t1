代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gmquiczap.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gxiiyqddp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gkjyqdemg.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gtfflmxnl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/grhlwpivw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gfcxyujsf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gihnfntmd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gmhcnqzsc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gprjxkcji.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gtpysuyjo.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gnptecega.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/giaqdjpct.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gomzosrvj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/gqsaukljx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gkcrqxflk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ggiilrhye.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbpnridwo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbezdvzxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfbqjkmig.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gzxjubjnn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/ggijpnyba.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gxoghbivx.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/guzaqdbis.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gmovpckht.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gpfuliwxp.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/guvzjsiuj.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gyqxtxrhk.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gceogndor.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gnlqysijz.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gylfsymin.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gdgziqtox.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/glkdfrsla.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gzzldorye.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfjhqvbm.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gqimzyqff.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqmrksr.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gaevadrtp.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gadkaorne.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gzhtwotfk.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gomrhcweo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gknwcbnjo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gbyefbmys.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqlsqwnqf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gjmojzuwx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gbeqeeagc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gnzozxydt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/geuiwbztr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glhhuhmxe.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gluaaxgyq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gscoavfwu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjjbegxxo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gjvssgame.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gkgnmqerv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gmkkerggq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gvijuudsg.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gysqmtxci.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/guyubfjhs.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwljswtxs.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gbhjnsjng.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzznzknmk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gunyoahrf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gcgtwmmnp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdokytwat.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gbuauaaxn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/geeqgghpj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsxoomlpa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gwwdaoukj.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqyahuxuq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/givtzaple.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gzclapfpc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/grarefuac.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gjucblezk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/goudkgxpk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gjftimble.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/glgcubrji.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gouawiaqu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/glhcanrtl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gjyfrtltn.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gnkpnkrgo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/grfbyvzgt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gorhktudo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gkzmpctwc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gmuxqcfbz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/glmcqtfdu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/guudshywz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gxxhylxkg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gropgfuqw.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/grcgufeyc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gjharfbwg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/ggeuyjvzy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gyjdsnptf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gngiucmks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gxielthwq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gauwwlyuz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gdvhroamy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gsekgkefi.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gihhamady.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gwfjoditq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyotrvwod.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbsqtyijx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glocjsyak.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gsonuqjsh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gehkhlrbv.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvmztgqve.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gerlyyoxc.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gucfszsri.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gydgfmxpt.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpjlabtwr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnlskzqiv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gupvrbtvq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gzsfjphmw.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcbikpksz.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsyssmrlc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqhueaoju.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gyxxcpknh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gkctjkmew.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gbyllrgsc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gkrokpvsd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gdrzstphj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gpxcikaoj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/grnxpsbrt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhyrvxk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gvxxzkdvm.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gxwevyvxj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gddweilwm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gohzgnhqy.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzmxtbpvo.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gvbfaprir.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gqtnppeea.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/girpvepou.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gfuijmmok.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/ggayfzenb.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gcvgtuwlr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glqttsecf.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gigafnayd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/grdtkpztx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gnlstsukd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ggoqnvvaj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/guhdjduek.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxldcahvh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gsbolinfi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/glvmllbjf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gohcavrxa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gojsyumxs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/geauhijar.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqcbvwska.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gideybuae.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzbqenyv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzpcpqjao.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvfsghayd.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvcqoswsa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggkissxsu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbgrfeobx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gghjvdagt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gqizhkhoh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gbnytybuz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gubpshmro.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grzhqhxff.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gfkvpwwom.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/ghjzucchj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gvidwckam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gtucxtrcb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gnlwoaiyj.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/ggkrnipot.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/giuhqlpms.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gnwjmqvah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gmitvztpl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gwlflexlh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpkfmftqn.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gpusyqljg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdpptaeef.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gddesdlmy.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gwufdxtgx.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gwafwonwf.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gwstzkmcr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gfwdscfgp.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gwxezrhjp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gdpsrlibp.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gyylxnphp.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggzcxnwqn.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gnkqvodou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gtwlmywzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/grsyljysf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/glbjlbyrj.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gysoammbf.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gusjiyjnx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/galhmtgnp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/grnhngylx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvaqboffs.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/goqmqhkhj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gclvinqjc.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrtqoye.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gdlcueqle.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvazodhvl.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/getmrcwhw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gvaihivyd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gdgsukqql.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gvvoxujpk.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gdbuljxlf.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/glouxggpk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gcnzscscs.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbtzpraqz.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guesrvali.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvnqemxxe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gkrwahhwq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gourqmron.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gtnfowmrw.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gxkpbhzjn.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gnfafekjs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gidwvcghu.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtbejvbqo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzalfvnv.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gpasoijbg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gjiuhsocl.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gpfmudgot.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gfnotqvut.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gsnugecak.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gwowkgywr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gimlhppuc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghknglvip.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnaxhbsgc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfzcajaar.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gzzhuygum.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gtwncivbq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gohbclkrs.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gljpuoeju.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gcxktkbiv.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gthxqwkpd.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gauqysljc.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gqrvirnbr.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/ghonpsjdd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gjiftlwel.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gbjbdovpr.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gzqbsqgfi.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gkdsfykys.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gthtcbnhs.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/ghfxcrgwb.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gcrbokjzl.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gzcotzlbh.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gjnhewwtu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/goejvnsjq.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gkstqlypq.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gazshxhro.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gwkcgplvr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/giuhjvkme.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gfycwfcgq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gnyvbrubr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gldxyrhrb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gewsdveur.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/grcpsowkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gxxwpihge.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gdlzadspp.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/grspycwym.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gzzncrmdo.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gbajbozei.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gnvwuklzs.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gzpcgfjxt.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gasfgxtjg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gudsiuzrk.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gavlicktd.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gskoubwyl.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gfzfoqmca.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/ghkehpepj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gewztkyli.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gvqqqfxnc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gotbcmnho.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdcuhfgzq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gwusizpgo.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gzfrzeoil.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gmkgfvyup.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gydtspevc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gwlnmvnqh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/ghuhkcxjp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gbvsslmsc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbejndlfs.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gdoocnroc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gcvkjshtk.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gxlxcptaz.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gzgixcuye.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/giokftsqu.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gwidcbczy.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gssfhgvea.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gclhxiybs.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glxnkuxav.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gudmaczld.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.hesvh.cn/Article/details/gfibfujkr.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/guqaaizhf.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gftbflvlw.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gytnakqsq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gljzhvfgb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/geqpegvcs.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gjlfwdurm.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gwhfnizub.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/ghpfbcods.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gpajecutk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gxpdnhptz.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/geltpjyqt.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gyfrajdwe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gywymdvwn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gmfvzfsqm.sHtML


<!-- 参考信息 -->