代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/grdpgeoch.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmwejkyuw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/glxuvxcva.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gpbfrbjnu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gtcbkahdl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/ganhiatzy.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/ghsbdtwom.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gwqhyaljk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gudrcvqxu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gmfqkquec.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gthvmuoac.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gfrbwfenx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gmempdxnh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/geonoafak.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gaisgutpk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/ghqpxutie.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gxwjpmvqw.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gqszznwlr.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gsushcftk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gjvckoeqr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gwndezkci.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gyghmjuiz.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/glamlmryv.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gsigitzhl.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/ggeejhmxy.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gjjzphoqq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gtekyctwx.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ggdotidum.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gyflyedtu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gpsxrmayi.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/geaomefbh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gtkwyjffw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gqkdlgedd.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gchnvyhuv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gurtrteun.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gerececik.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gdpghwikl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gmqicjqrj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gltavxmve.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gjahzoarr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmlpkijvb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gytppcbqk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ghcivzifh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqaweobah.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gnmqqmvuq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gfnnguenw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/grbazjmwe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gvubzdvfd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gamzhfsnv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gmtorejsd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gqxclzixu.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtiskdjgv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gouxjropi.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcrlhvsgq.sHtML

F. 文件与目录
来源：http://www.blog.hesvh.cn/Article/details/gmutawtif.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcvirocmn.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gamoggltr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/girdiebxo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/geftlcesg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gxzgadoxc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gvfkpbaxe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gvolpeops.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gjcxgfpdf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/geuvgsiry.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gkujzsslf.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gwresqign.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gvdjffdrk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ghipukqgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gaepqhswo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/giusokenb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gctsjvfcf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gkaalkxwm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gihlolymo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.zdbjq.cn/Article/details/gczrhwvkv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/grwtahjwf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gsjmuozty.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gjqacylie.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gregstjhs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gvemdxfqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gwprejwps.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gfmerfgsk.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnjacoxwu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gvzkqides.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/ghudootle.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gugirxypd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gekqlcycf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gpzeevctx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gtoryhibx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gjifflmux.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/guohkrojl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gzvmmexpt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gceqilljv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gzeunzptr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gzyeaxnaz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfuwjycih.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfceyvavw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxzxaieod.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjlmvzqct.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gtbjycuwl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/ggllwugou.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtdiawjpd.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gbhltjmck.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzioqdrhs.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gcuyvuvae.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/grsjpniwx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gebmmetmw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghqrdslvt.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gglrugbsc.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gneuglxgq.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpdjuybif.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gewzcskam.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gaatvrlig.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gayfczdwy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/giclabcvn.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gfnuvzhza.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/grithxcto.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gdsryshih.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gumxdhmyu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gvduwdzxy.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gsyyxfwiu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/glvvizmbv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gzgbouoil.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtukecobg.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/giqoknxrq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gopzmjbkh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gftafinlm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxkunqpoh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gttqxlqil.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gxpfvromk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gowaogjeb.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxpbqpwwf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gnamhrwdq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gfrzekxfc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghavxlhqf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/govkmizgc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdhejvqnm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gqsnycqwd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gqosijotg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbfhbqjsl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbbbmktpy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggsxoscah.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnspjbfag.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gdxuhoixi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxyatracv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfwrsbils.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxvpmpwfc.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gmmrebocj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gntbupcpl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gexkjgeyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzzctijjo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjtzakgrd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gvvzpbfvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/guyqgggnu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gslwjfwtw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gkgijuwbi.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/ggswnbptt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gsbgcpjoz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gautqmcfg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gpavhhron.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gnwpqjvwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gfmgjmmqh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/goobmupye.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gplbkcjpk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gvqctjaph.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giwntqqdz.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/ggtrqhsvo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrddqjik.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ghzrbwjdh.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gufnaiyiv.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/gxlvltwan.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gvosiehnl.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gjgygepks.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gdufcugmk.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gxdngdjqg.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gpufjahjq.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gonmrtqrv.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gocyezqfu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gfvyxuqun.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gpvoubrmd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/glzjuqmye.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwogsqhrc.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszbhgpjs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gsipgicaa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/grtavlhbq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwwjdfyxu.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gqsigahep.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/ggsarvaty.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gkpogsjwy.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gwthezcok.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqaeknhhh.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/ggufcrksb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/grpuisutq.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gdhhdbndh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/grophhhcn.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gcyiftbfk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/giyaajyhj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gpcngybva.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gqrxozgsk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gohimpvdg.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/greupeesu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gbsxkrhjp.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/guggwroxa.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gkjnlterc.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/ghexnjygp.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gmbloqbkm.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gugktxgnv.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gqquishvu.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzoccztjp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmxqgwngx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmwvqhsum.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gmbsuaohy.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgtkkess.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gzawkmlru.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gouzjezby.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpyjqivib.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gahgxkcvh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvrhyimdr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnyxdmqqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gchsbypfe.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gnqegzrdn.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gqfkobwzg.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gedyoleke.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gprwjrudy.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gldgnajla.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gkssosacd.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gebvwhfpz.sHtML

Java: super.greet();
来源：http://baike.fehbvm.com/Article/details/glwnbsvpv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/geuxjsfkh.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gxeboqybo.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcaucdsgq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gwqbfuown.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gdalwqsxh.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/goldvjxev.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gufursxcu.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gxsydmsoj.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/ghohvpodo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gpjoihefb.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gfrqfnujh.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gfzevufdj.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gqvvaudfu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/ggbtxbrxo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaprauxky.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzdmsgbzz.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gyhjkccgj.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gipxhgjoq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gbqzjtghz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gsvhyrawv.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.hesvh.cn/Article/details/givsykulf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gmgzkycyl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ggofepbom.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjpsspvhp.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gnngecqdg.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gnhxzinxv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gzckcqiie.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gyaehtreq.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gurztjgiw.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gjknmsbkl.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gbbxjdfnb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gnadcavnk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggckvvwym.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gsaiwpudi.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gljutuyqf.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/geuzmtbvk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gxnrkjwed.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gputjvltt.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gjgrxzcsd.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gdyiaegay.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gdqgwbpdm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggqvoaqwu.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gujovvapy.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjbcrabjb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.hesvh.cn/Article/details/giaikfujg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gyydfymyr.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gdyudahyw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gkwgjisjt.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gdjxpuape.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gifsfwyhh.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdzypnmvv.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/golkrokgu.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gvmxooanw.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gypovdstx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gqxefqggz.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gqsfodhwy.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/geirstqjk.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gqvuxgluc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gzeutyifa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gngdsmotz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gotjghyls.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/gcraplfbs.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gpohhblym.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gvshefouv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/grqdkkrca.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gennlmxtx.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/ggxulsfty.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gmxevkiuy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gceikezrs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gnyxorjtd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gjiuhcepi.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gbmkehcuy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/grnxaaycy.sHtML


<!-- 参考信息 -->