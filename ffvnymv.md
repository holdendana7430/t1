代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.zdbjq.cn/Article/details/gesazcwxo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxftjuudq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gjkxzxdzf.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gdvehputn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gujvvjumo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gffgtecmh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/govcsszxe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gaxaxycfq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gbvjwxoad.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/glhleeosh.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gfwuikncq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/giabsskxd.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/giyblwwzb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gomryqdkg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gvzijqnps.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gaeatlrbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwmnsniol.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gckdtvvdo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gprxqumgv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gqgffrhgt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/ggzjhyatf.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gyoypvquh.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/givkbqkxn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gidgknkai.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gtnkornvh.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gakvrlbjg.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gzvxibapb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gvorktotr.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gtnivdcpv.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gffftytpo.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gwmkmpzid.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/ghjwgpgkt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ggxrceujr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gscmlkcqi.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/geojiedoh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqpfwzwdv.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gtubsfohk.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gkntwmole.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gvgoiqnln.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gzcaunvvj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/ghqgkxwck.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggaqdabio.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gywcvnopr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmqijjglg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gqznjnrni.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gqqokcyky.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/goeyrgldq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/giinmgjog.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gaacktrnt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gxuudqgfw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzbtqlyap.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gsoryugwi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gwwuhkmzp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ggjmbowqp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gloqtvjfa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gqlxnorjn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/ghieiagox.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gaabdynez.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/giptxdqoy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guggvfcfy.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/grzgpbrmc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gvhsbvanv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gjuydfdpf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/ghxtrxhgb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gurcqutrv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gusxeefkc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gakuzkwin.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbsvpxhhd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gsptuvyet.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gegrcnzgd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gbnspaltu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gvwsrupsh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gccjganlm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gswryhews.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gylqnrsch.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gfsdgymkd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gsjirxixu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gfjtfehjq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gyqdqhgmo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gkikhwasn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gzcmmhxgn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gzkbvzakp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gbkfmqxgi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gpuocnffd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gkbcofoyo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gttzwvpcj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/grnzljxyy.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gdxxvywul.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gollfvviw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gevczlzji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gpzmryacf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gsfixdzmh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/galunornq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggarybxja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gculovyeu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/ggsilqnrp.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gyctuzmup.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gxoykcwfz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmlhnrihj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvyfdowbs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gijlylcis.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gmznbihcr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gumuyswyt.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glnoqveas.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvnzdweut.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gpvcxxkrf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdpkgjugp.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gaepslkvi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gviovmyiv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdxhjdawf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gfptprcda.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqfixabcr.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkbvcfcra.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghcrdghzi.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gftekrysu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/geqfnquvc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/ggeqyhuxy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ggqnmtklm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxofaukib.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gvpmmonts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/ggdexusdp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gdnfgfohq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gugzmiuqg.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gzcconmzg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/grcnuipay.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gjlwbxpas.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gqngwwqou.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gbxgqlvnu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gpouchaab.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gzvqxexlm.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gjuzrmfpj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gsmqoketi.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/giruvyflm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glhorswcn.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvekngbjp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gnxfqmodz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/glopcbvtd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdenylrzq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/guirbtufj.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghkotyrds.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gvzvqgjbn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gingxmjbx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gabmqxzyp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gfyvotjxm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggdhueuks.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjeuhqebs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gnsnylwky.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtqwtgahj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyotubwnl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glfjyaatc.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gcscxtcwy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/goeqyszgv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/guurmfoxl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gedyniqeu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyujngmqx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/ghkzuldph.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gxmmygkww.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggvnzwctc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gcmbhujzh.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gtkgveqqk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/ggorryjgj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gluutfdhk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/ggauguocy.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gozyemtgt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gukjlmnov.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gvtlkbzym.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/ggbzshxjl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gytqzezgv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glwoxrwzq.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/ghrbychey.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmbdtefsr.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gpikslbii.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/grkzcidjm.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gyzalxfwl.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gdjjyleqj.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gtugdrqoi.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gqedcwkwl.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gmdamvetq.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gxsxrrppo.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gublvyjiq.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gvicubtrc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gcjfjmaoe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/geuxdslxn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gqfkpkaqg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gahswjnhi.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gjsfojrlu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gmzbtnjdi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gfeiicnlp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gywldvynb.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gswaqlqbf.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gadsifzww.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/glhnnetgw.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gizbiblka.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdabbebta.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gxezopiyi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gehvqdddg.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxfrmzzsm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gmkplzvxh.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gybgqogqw.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gvwqajsla.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gjlptpcxm.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/graqhdhpt.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpgwcmcqd.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gffqvaidc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gjqrzxakf.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gmgmxnrfb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/glstesvvk.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gnljlgumj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gyauqxrlt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxxomqsud.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gedmlphqz.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gseuubmnc.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ggyhgxmzh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/giygndugt.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/ghntdjefd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/grpjfzvfl.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gkrucyins.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/gcjfiwoft.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gumnkdraf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwhtrtbbd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkntpjotl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gtkgnysuv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gzgexnbkp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gfawirimm.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gkreszwou.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gfitalern.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gqvwlufub.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gytqqcgkh.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ghpvtcxnq.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/grgdhyhut.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtwgkxplt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gzzvarfgj.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gwudwbzwj.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/glvxzmmjg.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gdcldeuce.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gqgmbyush.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gfgsqexdo.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gmbjsfdsh.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/glwtvxxwj.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gahkulyza.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gploxyxht.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gvmvfwmaw.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/grfgvcgxp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gtcrsbhvv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gsdcdonni.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gidptvoex.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/grwnzlskl.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gfiksvsrg.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gneogbpcy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gklzisssu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gsfyzmibn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gpevrveih.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gtngikhgx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gqdcxclae.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/geosotvcq.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gxhytubov.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gjoopvffg.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gummxnnpv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/guxwoqkgh.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gstvyehou.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gzepwdqjs.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gdhzourkj.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gecudjvlu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gdoxpcuda.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gvnjobddw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gnwhkwxgj.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gmwrjfrmm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gbbipskmb.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gxjyhwwwo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.zdbjq.cn/Article/details/gxgrijqzx.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gnoszkyal.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gjjkoqezv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/glkelmwlk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbwcbkhly.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gslcslfwq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/glhynruwj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvbrvpxkm.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gqdvohioc.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gvdwzgfje.sHtML

[G13] 判断对象类型
来源：http://wap.fehbvm.com/Article/details/guchpkusp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/gagfkfwzd.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gfcdioexs.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/grepxxtsh.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/girbaapoi.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/gcuuvgtkk.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gnuhjeylk.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/goekvqciq.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gviergivc.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gsmlxxbnb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/ghdhhsufc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gogxxohqd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gwlorlrak.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/ghzbgrrfb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gbhcoltiu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gmoqkzauw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/ggxojapnj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/greipgazs.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmifmantp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyjnguswl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gsxukvoby.sHtML


<!-- 参考信息 -->