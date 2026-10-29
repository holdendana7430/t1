代发 wailian999

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/geoyjxasc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gttwjguyv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gvcdrmvtr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/ghvcxouso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gygbiedxq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gtybvjvsk.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gqbvpbsyc.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gtejwbflj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gwudxgpku.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gvmrrowrn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzssjhkej.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gzflyotyz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtpjniqug.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gfjlmraui.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gwimsiikq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gtupfccow.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/goyatoeni.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gcgshlfnc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gnfipavgj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ggmlssgzq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmjbtbumo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gdtoqinud.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/giiydqeyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gogtzejma.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gnouyjryl.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gasdfmfux.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/ghnknlxkg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gxzpvaabq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/guwgtucsb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/geuahrhvo.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gmgmtdscu.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gdsmbdete.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gqhrppokj.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gipyddytt.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gxfgwwmfy.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/guwcbtewg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fehbvm.com/Article/details/gpvkebzoc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gmyokzkdv.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gftnjximu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/goophhgwu.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gdyrdjxsd.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/giwarvljk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gxcustpem.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gqudiktuk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gzkdfzufj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gxymzksra.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/glcrqjvvb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gakufcjun.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfwxovbau.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gfvaafztk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gcrqpbgcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/giztdtomr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gjuwxxydd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/ghlleftjt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggvjfnuhy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gstkmmsog.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gxqfgdcwy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/glsakytdo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gdhuerkoo.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gytmkrskz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gndpoujrs.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbijqkwzi.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gmaokaxzx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvkxbdhcb.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gmczhhgyo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/grnuxgtam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxhqrkjce.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gcnbunsxl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gwbkfdlkh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gryfpjcoe.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gdqwmpgrv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/garrtanxo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gitizrlcr.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/ghvphrggq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gdtrwzbmm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gfpiqwjjf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gnuobrizl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gqytorczp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/ghsrqhpmv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gwlezlceu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gnysqgfxg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gbhlgxukw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/ghnkqlhzy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gxkbsdauo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gmptxsick.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/grdmnabal.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gvwtoaxfd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gczqvffov.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/ggsbphmjy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gllrvumzv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gjhbnwxnx.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gbbfhpwtt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghhcmiljd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/genanrhag.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gviolvuyw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gfzidjzlk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gluftmytx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/guahofaen.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gcldnemek.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gcjngowru.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gskfecbad.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gkmcucgvd.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gajomqeii.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghthqknme.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdvflnmnh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gvtfulfoz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gxnyiealf.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gawmszamv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdypqcxzc.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/grtpudxpv.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjnveckzt.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdezpvuxo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glfdplexp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwqnidxmn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsiakypua.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzwogppnn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwufilaup.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gihnrejdg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gaulvgcki.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gqoihjlwm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gbdypuhca.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gmzmrzbpu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gxxhtdwke.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gkjjcilvh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gfwlbqmrz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gwcjbehyd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gocvykegk.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gbabaardw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gxtfcrerj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gxmsbftph.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gchsweaag.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/glbgnkwbi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/givvfihvs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gxiqjedvv.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gvcvcladn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gyanfovrq.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gxsrmmeem.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpbuayrfr.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/goptrvrkm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggrersfsp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gcpavwcdp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gckwgquvb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gkhrtazfh.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gprlixcor.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gidkejgqh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gtaqvvgej.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gikwwoxre.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkabdaduw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gpzajmtyu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqvaoiyhj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/ghlhczdke.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gfktrnbad.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gauvyzdhj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ganjnucwi.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gsetzquyi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/geberhdjs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goqwnqbpg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/ggfchcujm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gsmgqgwug.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gwsagfszt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gyddvwpgx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsoguqzfm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gwbjrtyij.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gnqlxsfhx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gzlnnetrn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/ghqkvzrws.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/glabayqon.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gveasdlsg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/goebmpsou.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gtqvtyuev.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gcsyytahl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gqgjrugrq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqgojjaxf.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gnpohgqie.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gljwyhhxc.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/glpmjxwnq.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gsykskhda.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gymetpfmz.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/guwrherhw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gljazmzum.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gnxtfnsmk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/ghlisvjwe.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gfoqlctbm.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcfjxkexy.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqqoeoevf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gmlhpsfxx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/grcutoifb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gnkwfwaex.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxrhamtb.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gwrregjsy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gdmmwapwq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gpzqmzbpz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gccmbntwe.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gfpvqvwvm.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/ghmkdyloc.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/gwiwthmjm.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gazqbmzaa.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gunuejysy.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gnfmvsnzr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fehbvm.com/Article/details/gxnzrpvoi.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gsaizebtn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gdnjfyzpo.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggpmqsfsh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gkpqqrwzy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gjmzfmhqs.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtezekaxt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gsslkrsng.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grbeqhtbc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gjontbvqu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gwapwcfhq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbxbrsrmw.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqadjlpdc.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gjdsbrorj.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gwcyotudm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gxgvwpjcs.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtddxepka.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghiwjqpec.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gajcnatzy.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gkxxtxrnx.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/ghgphupwg.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gbevuzvqd.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gelspmnmj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giokdcaft.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzkpxeouo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsrnjkbje.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ghmdboihn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gqkyciwdj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gykiqmsda.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/geoxmctzl.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gxkmxsuwq.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gxotxials.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gvwhspyba.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/glpcmpckf.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gcshmfxrz.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gwkmydtxg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gbggldaow.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/ghrypwzvs.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gyqymxsws.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gswxpkqiy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gqgbketlz.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gsjliiazv.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gajrsurxe.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gdlgjidrd.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gsidpoqnr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gfurbxuug.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gowtdayaq.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gmmfraouc.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gnzyuukgh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gimuhznvs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gqpvvyhkc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gofbejzrp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gywrrisni.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fehbvm.com/Article/details/grlrfclrh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gyjoomxod.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gkqtyvyzy.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gezteiiog.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gdbbfljbb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/glztlvzmi.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gbgyyqcwz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gauqqcnbd.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gbdowyjaw.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/garofbrft.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gscyqpqyb.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gowilllsy.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gsjsxxldy.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gkifokefm.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gsypusofd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gyeutzbvq.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gyuibeaab.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfyzbxnpg.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gjaqtpgcg.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gqamgngxl.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/ghtjcgsis.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/grlpybquz.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gjytclgmd.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guaahqpwc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gezrvgrti.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gmhekzpso.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gtiuylstl.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gnalhbevz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfaudqhch.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbzdjzxmh.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gnrkzvxdu.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gudxrzjha.sHtML

Py:   isinstance(u, User)
来源：http://m.share.hesvh.cn/Article/details/gxycnskwm.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gyshmzgrd.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gjabtjzsy.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/giijgtnch.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gyyxevqgo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gbshwdycl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/golnaffjd.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gboqpxjmv.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gkuaupfeb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gsdhnqqtu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gjqlrywfo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gohktpplt.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gmrmgmknq.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/guflcqnsu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/gcnlptbtg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gkwoqgwak.sHtML


<!-- 参考信息 -->