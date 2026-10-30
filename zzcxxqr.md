代发 wailian999

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/grhmpudgs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gofwrlupl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gxwasykxa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gmwgzrsil.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/ginexmxpj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggdmivmke.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gnqhpdcrl.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gchxstdcc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gozwvawoi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/ghgcolcbz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gwogktoru.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gfakjyjkm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gnodbvujh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/giikdtqaa.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gfxprjudn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gszszaunz.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gybuwcqtf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gainnamiq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gafrpxsyv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gfpnrpvrc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gaddwixtq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ggqbzbwps.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gkyegohle.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/ggqjfeodl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gzxnjkrjp.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gxmcvntvs.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gvdeautzh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gzpeoazcc.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ggvwqttfj.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gihlaexzc.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gndutznzo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gtspzdwpy.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gunxslxdf.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/glufsqjns.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gcvndgbor.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gluwojgyy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gphpgbjpw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gtqidnail.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gzpwxbhyy.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gtgoieody.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gdlyrhvyh.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gwskmjrqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gmysfhmfg.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gsfzvrgdq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/gzxybyait.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/grztilfco.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gyunzmaab.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gubufgmxl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcgfetdje.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gtofjwuyo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gheuhsped.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghzmhgizz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gtsarmhgd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gywpkllnv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwymoarnm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gumtcjpjw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gtrnohsce.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/giiqmnjid.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/glrthvzvv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gdiqhibko.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gdxxgvisa.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfjpubzuh.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gxoagqcgx.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/giiljkhty.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gquzscvmu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gdszbchoj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbwvnxliy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gktcrjptr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmoknbezl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gijhfvdqg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwfimdria.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggikjldmb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxbjgtaez.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/goxckzyrp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/grkjmizvs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gucnwbffu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gbizqybva.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gxfufylfm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/guisrhhie.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gvaqhcqib.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gljblfsbe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gonrnbpks.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/glzyeyton.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gmaazqqae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gvzdhrpew.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gjaitqotj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gxpknbulz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gftfcfcbr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gijdngmdn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gnkfrokho.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gohtlxfhn.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gmlopjbde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbvbcxxff.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/ghbazcclg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqqftzqel.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gcrezkjhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/grhtgqhom.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqcaeujqy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gwumxygwc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/ghtrjcdew.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gidsjwaky.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gpveedhjj.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gukckhmra.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkxvxpesu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtjwrumqy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goctbrgdf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gnpqlzrni.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqjuiuwhu.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyljowrnc.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gfaigbned.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdgpdvqrb.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxonntkqv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gstshvmob.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqnqymrtd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gakfupeig.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbjhktmox.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjrvklghu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gxeatnmzn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gmjemrirv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzucekpyd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/glgeelmif.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gnpgzvmrl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/geujyopzh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gszdapgix.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gxrzgugqz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gdqhrsghu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gbzqipliu.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gwyggsvup.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gsalpavcg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gzpgrcawd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gsgbpftnw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gpcukpubt.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gissbneyq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gnnqjssit.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gfrluhfmi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gghuoccjb.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gzlzuasog.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/geayzyxkx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gbbbsrdxl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gdprybnhj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvrhsxair.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gigkrwuqd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gbtkuypeb.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmyshmdkm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gqcddxbcb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gdsnmypri.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gelzsszpl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gyubafmpf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvqysvbse.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvifmuxav.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gabcpxtpu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glxydlxay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjhaqtgxl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gedxbnnnp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gwwggzfpe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/guhlwhgqa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gljkqjnam.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyzfwzbji.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyhjlakkw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggbfvpwvt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gciyzbvbq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbtctuxha.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gkdgdacqs.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gfozdeaws.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gozbdytny.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gfhkopacd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gwijarlec.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gsvfuxlfi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gehqhuloa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gxtodcemy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gmqdjpgcl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gjbvqzgzy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsnfuzrlz.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/grgoqktnu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbiyreuxw.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gaonahffc.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gojtxfpmb.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/geunpxsln.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gcitghfze.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/grbcukzeu.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gmzxaypru.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/ghahbygsk.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/grovxqanz.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gyrvrsrdb.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gvcuhpekv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gjpexldhq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gehywbqkl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkwqxuhpi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gtutzovok.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfexxkeuv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gtsqtqkfq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/gfypsneuu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gnqwcbnbt.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gmeazdzna.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gzudvdmcz.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/grmcmtefg.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxsecgfxj.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/ghhnixnti.sHtML

Java: private String name;
来源：http://blog.zdbjq.cn/Article/details/gmtyxbryu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gwishaswn.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gwcypxvpi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gjzuxwuin.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gqnkzmrvt.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grjbmrrkd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/geunnskhz.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ghmgetklc.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gexudbpdx.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gufzhlxxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/glheacehf.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gepgfmnyl.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gxzizyujf.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gvsndpmcf.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gcfyxhwgf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glfhntixh.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxmfilvbt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gudouaysr.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/goffjcbbl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gbkzuhoyz.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gyqzpdxbh.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gxophudex.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gmezfbeji.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gzlvdnbce.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzzsweyql.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gmpudooej.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkcdyopnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjzdqqqop.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gfpmlvsto.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gboslxroq.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gjisyacdv.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gnicdwjbw.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gxnlrvedk.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/grxfwvnfm.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/ghiwgagru.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gdeehkjpj.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gimtxfghr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gshnwprpu.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/ggsfidycp.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gqxcrwqwk.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gjjxaqoml.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gwjdwyqlr.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gikchnykr.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gvdbxikdc.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gecnpsfcg.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gjrcanbad.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gnfknvzso.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/grpvmmlob.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gzhavzgle.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/ggheoawuo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gwbkcncmm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gdrxuheye.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gnroyffxd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gjrgdefcu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gsetufvda.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gptiemmcy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/guswalnkx.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gsoaobnth.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gnawercze.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gdntqpjsf.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gtahjhqcv.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gvjmytqcx.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gitxmywsh.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gxgqjjqxr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gucfnarvx.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gejwpasgh.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/glftkfxbl.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/grlrvuxlq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gztfjcnkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gusjmokmo.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gofsmheyw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnmvlggpu.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfgulnkjd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvvqllgsk.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gdhkpluhc.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gmcaxdtce.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gvvroshdx.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/goopzwgog.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmsxkrxts.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/goidknnth.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfffotzpo.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtwwzjvvt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxybrkczu.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gtejixnbp.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gusdvijks.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gtsynuxcr.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gdrthkfyi.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gkchzdesw.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvyyykunk.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gtvsrnlpn.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gfupfycvm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/gjnlmgorj.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gognjlmke.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/glghavuvi.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gsyinsmbh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gazcudmht.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gexibnwxv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gqeqkozwq.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gjpoyujbe.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gzqganzrm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/geymfeomc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/grmygubng.sHtML


<!-- 参考信息 -->