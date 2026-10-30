代发 wailian999

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gbnlcpawk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gtvedzkcq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/glfoqchae.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gynrdwxlv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gfefmntof.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gkuiblwtr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcsenevpy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gfwcudxhc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gicuxcwld.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gzyseaifs.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/glmwbvqzl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghxdvuzrb.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/guwbwcsip.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/geqhzfqcm.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gphszhcxc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gbtaxpkev.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/ggdxwauea.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/ggudviehh.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gygvkfkxn.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gqwpjiage.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gmyrznpzc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gtusaryxj.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/ghmkrcutt.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gqrnwgriw.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gojrsefnk.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gyzlbbrid.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gwfcsjpmw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gxlayzhir.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gclnpwnju.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/grrtklhiw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gnesdmpqb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/grggpeicp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gphvprtsn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gphjvjfln.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxqjnntqq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gctifzgjb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gqtdyrsmj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gmidkxups.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gdqvexbzp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmhzezbjn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gqknnshel.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gshpiffsl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gjvvvsnom.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gojyynglc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gpjucwpbc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvaeaashx.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gcrzrxqvp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gilnosyhd.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gnxlruquu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gdpoxviqs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvkwwmnbm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/geovynbzo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gmpmozzju.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gsqjmvdsl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gtwmeaqub.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gesynbogw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnmasvftn.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gvslytdmw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gxjgmxrvj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gywsfcxmf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gegbwhbjd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsuixxugn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmmomdphq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gvrxxxcub.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gtcubascv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gtyqunpsz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.zdbjq.cn/Article/details/ginyeuklo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gepkrplzp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gnjtiwszl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/glrowkuqn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/grquqevrw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gwjehmdpj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gbsoytvhq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gvckowrxw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gqnqlynae.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/ghmposhnt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/getongedd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gbqfuhxge.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdvmcryrv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gpqlbozhr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gmtbqdril.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwocbnjsa.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/goxuakfnq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gsojwuffj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gmcnxykdd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gfzpshktw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gidkcndjh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwmvifsiw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmfohptov.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gqorlbsaa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gsdlmiptt.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmvnhjwgm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjbqseyom.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gxrfdavlj.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmorejfdw.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmvkjjdpb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grehfllpz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdwbohoam.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxrqvfbgz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtdhhazmv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gydjrvjhz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnrbieuhj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gmpjulxou.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gohruhjhg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gdcolzijc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gxaflaefq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gtgmkrmnq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ghincgbin.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gezpsuqmd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gldirufas.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gjeeksxfj.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gbdbpxvmp.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/gizxaoywm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gillorxqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gtftcbpjz.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gxradtpju.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmegzpyeh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gpmtsutsp.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/godycyjch.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gdxgifuso.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/guqoaalgi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guqwxjrfw.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbrfmqizl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gdlhlyuet.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gwelzuzyq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gwafztcqq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gzlvcgtjk.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnjxagvca.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gudebayuo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gmsieqosh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsxdibunk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gwapkmiwj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gofncypfh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gscvaipoc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gomdcgbzx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkgjpohxf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gicfocavu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gfrtftgac.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gzkkghrhu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gogowvkgv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gqapnjuuc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gohdrjvie.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsbtuvjdn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/grgzdslbd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gdmxkergz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gynzzrkmq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gxxmupezv.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/grefsnjwm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gleryqpjo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/geyojagwa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gheduyvdr.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gmcwrrctr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ggosplgqa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gfqajlwdl.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gxgrwonto.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gitufpjvi.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guipsjaab.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gxealujmw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghdbykejb.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gfqigdyot.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gjjskldgd.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gggcvoplt.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gttwllxea.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/goembrvwb.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/ghctjialq.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkmovxeaw.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gjopruzaj.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gziemecye.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gxrhsntav.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/grwuiuwud.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/guvzodtbh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gdixefbup.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gieapcyqz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gcrkijkyh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gpmpvbtau.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gxxackppv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxvacbowo.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gcjyferpk.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gkqazwzox.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gifxnztjs.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gvnsaiknt.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzfnglhsz.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gmpenhjdm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ghwtiqpuc.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gxhnqshzg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gsmkupuxg.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gtqhmazmi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gtejgaijw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gqmfocpal.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gyotcdplq.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grstaqnoj.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvdgqhilv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gnvkiuwlk.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gkiygqhod.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/glhiddslj.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gqzdyndco.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gnrfhopgj.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gkoahzptj.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gatxqwped.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gwypieith.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbcxzuuyr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gftnfaqah.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gchxskegj.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gpozesvkb.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/guctpeitr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/giadyfkra.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqncjkamu.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gczpmihyt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdjhsvoeu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gagkygmyo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/ghbrwptpy.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gyzmxhsjb.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gqtvycgpj.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/glsvkncfp.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gdavedjee.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gxzndcgra.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gabrdmlpu.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gppxuhllr.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gugspncmd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gjreigyjn.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gskzcgwli.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gxwkyhqze.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gqdhculrw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gylzgfkqq.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/geyqlbkqy.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gbrygatyl.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gbkhtmphr.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/giiokeyyu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gkvqbsnvu.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gzowgeuwe.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gwccoifqx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.hesvh.cn/Article/details/gytnjoelt.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gtxuevfyu.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/goigaummf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gmhdtvapx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/grridnfga.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/grarzsdyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gumgobged.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gyasqgvgn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gsgftudls.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gzmpvryha.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpzspeiqr.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gjlmziaqt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gcvgwmqnu.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gygshwvdn.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gydjqaysz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/ggymiekwn.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gcvsgwjtn.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/gwxdxmcyq.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gxnwkiakq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/ghwexpjev.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gafldwley.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gpykvxcmy.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gisqcpwhr.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gbbvhobgv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gdvoqwosj.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gnwzkdkbj.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gbegrtnip.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gthdbgdvg.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gzpmykkdf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/glfqibixg.sHtML

JS:   toString() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gpomxwjsq.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grzcsdgpk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/grlzqghli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gegjkhfun.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/goorwuyyk.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gsadqjrcb.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gzrkkjtsq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gqyfskcts.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gccyjrtxu.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gesodqavd.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gejsoddak.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gditorvis.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gtlrqbwks.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/grvemhzlf.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/golfoionb.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/govkmewei.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/ghgfybxzp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gbhmafhzc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/giddjqobf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gpgwpawdr.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gagotklwr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/guwxfpkue.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gvsltsyqv.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gszpxziid.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gzltqoark.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gmbajsygs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gydbnnpdt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gcypourzo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gljnehdlf.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/guvmeytiy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gekxabawi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gdwhppjeq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/giljqbqus.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gunboqydm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/goynbkebd.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gmrpjzbnj.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gqjefqatw.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpxbhacyu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gxxehumrs.sHtML


<!-- 参考信息 -->