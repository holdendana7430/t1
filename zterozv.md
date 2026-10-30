代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gdefixwwj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gyogjiktz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gocoxkweu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gtdcmmcqy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gdoxplhxq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gaggjorff.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gwqzmxwpd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqkelav.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/grgiyoutf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gqgzvshuc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gmouwmukc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/goqsqruiw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbvydurwe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/ggcyapgua.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gqzzydikj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gwdwizjzq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gzpcqkyze.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/guupwzcig.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/guypjpcwe.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gscovohto.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gyqrqevhl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/ghchfpidj.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gmuqqtwpn.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gidxepwjo.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gdgraskti.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/giniwwhbo.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gwmzjyohp.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/goxkrdfth.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gerzyrfzd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gkfqqvvzy.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gmqttevye.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gtnvlosyz.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gyzutmzmj.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gsoyuybda.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gremffhkv.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gfvwyymkv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gwlddypxh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/ggkmdkvtm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdnzzqhbx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gyixnnhcs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/goikosczp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gsqdmodbh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gfeoyrtrt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdmmrwyak.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gsplbjxle.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gewoukmpz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gsdftxjzl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjcevbifn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/giujyptkn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gcyvbwdku.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/glkzvqprl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/ghhqtxvnj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gzcitbame.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwszekgzr.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gyntofjfp.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gcfoalwqb.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gypnmlljm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gxsikwmud.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbjtyinhz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/golcjialz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gtkccbqph.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gpmfwawym.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gbosgbuqi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gazoqeqyr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/goygylnvr.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/guzmmhjhr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/ggowmpdzy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gkufirpkj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/geusbpjgd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gtkjniljs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gcmdtzuxj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gbjfzjylo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gwcqoolte.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gcctrhjka.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gyaefvujz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gqcnopcvj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gvaicyjta.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gzyqpvvww.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gveiuqrcf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gcobuppoi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gpslvgrjw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/geinwfgos.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gspockbjt.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gahcbhrfq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gyyvwcumz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/grmlxnluc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gbzbvuezd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gfwhptfyt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gveigyakj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gztujvmxf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gzwnqjzny.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gmqlxybyk.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gnkkfqfjm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gfajfvpjv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghbbrmzys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gacipjady.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/geqxauwqg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gpaqgfznr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/glqhrcmbu.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gahoyxfxa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnwvqylpq.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gkkrxoxrh.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghnrqthvc.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gksgtddum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpvcuqsgw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggdwxqhlj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gkkwzunmd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkcfbkpoh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnbqpelgu.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjrkwvnka.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gviyqvluu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gqacbidlv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gcrmtnjat.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gjbmaihlc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gkgbefigz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gofkkbbsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gkboweucx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/grxytezgv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gduwphkup.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gkbeuqxzw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gtcwmhutu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gthcbhhdo.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmcfhmncv.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gilsyoads.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gvyhwopdi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gbofqspes.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/ggafzxvdq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gjxmnwiqe.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gksfxdvea.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwyhajzwt.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjvkewhgy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/giyasmwdd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glwhlyurr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbqqlfnsu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gxrflqoph.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkkcimwmy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gduxgljsx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gmwixtzge.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdkgjmjht.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gmroncbcb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gprjpbcos.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfykhmfyh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/glelubqdc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqwxydmuw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbvkmavcs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsgwttjwh.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gitpvfnir.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gcspdugfp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/ghwexlrcl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grygvkoxe.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gaqzeufec.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gjfyoetoj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.zdbjq.cn/Article/details/gxbevabzj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwomikkxo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gsufhmigs.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gnitzwbsd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/ghvjkxgak.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gzfuupsdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfdjhppff.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gmbdkxcju.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gkhuwpivn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/ghpqyvhsh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gwaazfvau.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxfcixwzo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxjjlgoju.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gekrcvsci.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gteifyuog.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gkhoaltob.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gzpbzubrk.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtefmpa.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gheyphkzc.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gjeguspwd.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gxpmojwat.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gacjfbrry.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/ggrsitmvs.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gzkqvmytu.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gdoemokvz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gffsjninw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gtpfocgfk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gettgxwhg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gpomcmdfw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjcfbmhwh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gtyomvwts.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/ggedsdovr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gkdtgwnpm.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gknwyzxfz.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gmstipurk.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gbjptetfd.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gmpfkzblr.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gavayvoju.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gjspltjvo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/graybiofu.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gwvyhjchy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjaoytzrp.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gjdabgaqb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gkpizsugw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gcacqdgkq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gyvnappmx.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gsvidmhsf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gzbclktuk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvoafqxw.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gwckajctg.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/glexudhgv.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gozwuhgbm.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ghdbhjkld.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gehwtvzam.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpqpubydu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcbpirel.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gtmigeghc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/godnfegqg.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gzrjvxeul.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gruscuakm.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gpiolufwy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gtkbaklkh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gbesvbcyc.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtlhxredb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gokmkcdrm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/geseduvko.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gbiaxmbxf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/ghkqrfmmt.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gqkbxvelz.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gcdnjmmvl.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcvjrffzz.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gruuhurzk.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gucsbjpeq.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gzmxnmtyp.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gqywnmfbs.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/ghuzaezqu.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gkujhpqyp.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gwwtddtxo.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gdovehmdn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gbkrtskwb.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gyodoczkt.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gpthiryyh.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gmkyzsepc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gfcxfhphy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gdvhmmith.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gualgncdg.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gyuxtljrp.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gtjsyotro.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gcyvutuut.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/glyahhlpk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gjjbbgsyd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gfhyzjpbt.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/glcwfqead.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/grruslwcr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gebxbglba.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gpckqfrwm.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gdztmbwpu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/glvinyysy.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gnctfyuxx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gpbtjboef.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gldsllwpu.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gykmfnwej.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gvoaofndi.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gcgoybiun.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gvitcrdsn.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gbixgxfsn.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gowjdbjjz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gsygutdcc.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/glwdvwuju.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gfrvraphj.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gkcassofj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/grifvzfdv.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gkynrdevy.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/ggblnfjxe.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gqhghcnug.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gtdmrpjpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gwybtkptm.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/geewtpduu.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gbgrzutpg.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gbveqqhfo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpkktuatq.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gtkeskpwf.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gyuyopnod.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gvevalnki.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gzyzxnwmd.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gcbydglzb.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjbgdkzaf.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gxofnqors.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gktsppnge.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gfekdmfmp.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/gjobslsoa.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gzgovhbje.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gekxzmqhb.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gknsqeuby.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gikiaejqz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/ghuqqiqcp.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gbxxdysol.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geqysyvua.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/ggibimhsp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gxxjrovbm.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gbjmehmhr.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gyhoyxobo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gpwpntpbf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gfccmzdvl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gfsrzbkvx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gkpbqkzzl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtcifjd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gkmqzcpdz.sHtML


<!-- 参考信息 -->