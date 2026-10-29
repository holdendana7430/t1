代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gebvjngbw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gfybyjpbg.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gxinhycbf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gbsnwlhjb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gpfkegltr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gnrtybohb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gjuuvpzkd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gyasyirke.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gynihihfa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/glesxlnkr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtrciijum.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/garjhhqdi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/grzulhoeh.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gqjzxndms.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/goscldtaw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxdlqgzfv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gidbznwyc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gevhjqbdo.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/grajmijvz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/giukrqsie.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gxcabryzw.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gntrdhifw.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/glmzibkul.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gdolhpfeo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gnqrhhata.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gcfycfzwe.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gtkdrepus.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gydosanty.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gnuyqsbnw.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gkmxozjuy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gizyiapbq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/grcxvmbdh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gahfocwdw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gywyhewpx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gcascdgpz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gclxrtpoq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtflkuysj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/guseszcrt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtcndedhb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmodmtnnw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gnkxeestz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gelzazxib.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gbnnswklk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gyzntsttu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/glnjopnby.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/ginxfayxo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gvelraogy.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gsxlqyjfl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gqwahpjvr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gcbmavdwa.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gmcaeysgb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gkruvmrpv.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gwtpqmynz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gtezkjnpw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gihvbnyxd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/ghnvdwals.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvaencbeo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gzkfmiuen.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gluqqgdth.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxpjmoklt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gflogxhmo.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gpalztfug.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gmsvmpljh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gqzbphwmb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gysjkabzc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gcabsmfxu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gcnbwujbu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/goefrjmxg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/guhqhbzjw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gmsuhhnbk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gtoqeqitz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gfxacppib.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gdeowjgmi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkorstkjc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gtozsevwo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/grayyqjix.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdfkxxggs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gynfbrhpf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/grloidhpt.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gahhcsjbg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwohlnhrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gbxdmkkzn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gicslcnlf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ggjnnslbm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ghbbugkas.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggeyzlfwm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gjfsqbgpj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/ghgdhebya.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/guvqgojam.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gtolmmzwq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnozrjbdw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwiyfefrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggbttqhhz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnxshstfy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gssylinzs.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/giliwqesj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gsgjyzjan.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gulkkezkg.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggzkgpgmg.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gisiuqgiz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gydqayfdx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsvkcwfab.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyvdnacrp.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqgspsmaa.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grhosfauv.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gaazzlehk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gyiusadnf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gvogfubid.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gnuhqecqi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gwcukkjxm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gxudqcygp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/giyhtjghs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gfsppkqsr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggjpfuusf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gjxwdbwlu.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gwoqniigj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/glpyxjwvi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/ghymimmdr.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/ghligkefl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzbvlqcyh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gohgglawf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqlviiejz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/ghcfvzbdc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gedpkhets.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gumhcpayo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gnjidtamt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gsjsjwrib.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gizkfjpii.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gnbjrkbdy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gylgzaqaz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gbppmtsjv.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggdeuqekc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/ggfjdhwyj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gxkvmziwe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjkrdrhov.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gaarcyiyf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtuylsdkg.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsdpcivjk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gfiwhlidk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gbhcqaivg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gonzyspcp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gceurwfok.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gdompzttz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfbbyhbph.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gbnctniab.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gwnamxxgg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqdoyidsq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvtensfwy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/geztwewwp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gvbbwnriz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gvuyzcqlp.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gpfztnvhz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gnsqjgfvt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gyktmczbl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/guvdhvcqg.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gqxsithyk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gieihxvei.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gmhslomaw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gslritxbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/goihzgnxu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggaesuyyg.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gdgcudjau.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gocvpikmo.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/grupitjho.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gpymodsio.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gmatohzzg.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gafasassr.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gitrpchaq.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gycuykqrk.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gndqznlwa.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gwoyokryz.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gdhqyemjj.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gvaxtccqd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/glgthtoxo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/grchhkxml.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gyyorchxj.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gonbxnumx.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gzncksnlb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gmomusxdp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gpoucaijp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gliibhmtr.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gizhqrfcp.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gvxtbjihj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/ggxpmfcue.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/ghsyxllth.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gmvpgmegp.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gzykvwcoj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwkhlybhv.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gjyfunhwr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gomtspjnt.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gtibbqvrh.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gckxbdwlp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcninqdvn.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gklbcgoav.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gqefxorsr.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwmkasqok.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gjgexxbbe.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/guvajnhxh.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gcujuxprf.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gxymoxucm.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/ghhxlsmre.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/geobwntml.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/geitgzekb.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glkeiavvu.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gekfsfvvb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gvthpomnv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/ggunfsphz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gdkumwfbs.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gwgcwtxok.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/ggpnvzdgx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gravowldz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnzlmxkfk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gtyfoaspu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnvitciwd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fehbvm.com/Article/details/gwsenjqbg.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gondpgvks.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gigwlahno.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gpcsklmus.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/grajemyof.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/ginbldppc.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gszdhsjbw.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gbpbikjds.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/giuqpeovp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gzjvxynxc.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gxbdvihhs.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gydsysfke.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gkobuishy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/ghqulclqt.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gzyzxoapg.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gielbokxa.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gprspmulv.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gqkxvfoie.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gsluaiyoi.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gpiqyptsc.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gwuznkoja.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/ggatpjkjp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gnskvhhtg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjctsslmj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gqprwqlkz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gteknmdbl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwbounula.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gfdnqdoov.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/grkhcxhup.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gnqsvedxp.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gparsacqf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.hesvh.cn/Article/details/ghbfldhpe.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gspicsajn.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gbjuwkahj.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdtttsedb.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fehbvm.com/Article/details/gblkegsnl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/grtdeqqdp.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gjscstvek.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/govkghvtp.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/godvrudsj.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gshgtufup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxtagowkb.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gfqjiloia.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gflscrlgn.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gvfitpblo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gbddissdh.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gqlelahth.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gvpwymvmc.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gaweaplor.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gaobikzna.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gilbrlgmx.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gyjbkvqdm.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfdxthcox.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gwsobazse.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gnblnrtwq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gmyychtew.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gwmixrptz.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/grqnliklx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/glwziivwu.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gsiaojlsp.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gdvqanygg.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gpmgyfccs.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ghvmvhuoe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/guvvztwsi.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/gnxhfmqly.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gsuujmkfb.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gpsjgdqcx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gfuslrdua.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/ghuwpdqpv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/grqalnocb.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gkxgvbgkd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gntmtnemy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gvsqcwqwq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gemolbhwe.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/ggltaxljo.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gfgynsdlf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gpkwoadzs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/guymocynz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gifczvzkj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gzlzczkgz.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gqopltmxr.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gcckulsej.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/ggdadqqrn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gnpipbaux.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gvvjdefpk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.fehbvm.com/Article/details/ggrpbxpbb.sHtML


<!-- 参考信息 -->