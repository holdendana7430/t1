代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gmtliqjye.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/grqdutqlk.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ghocvkyuj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gvjkgnajj.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gjmqjqcap.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gjbreorhc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gtxikorvh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gxbveudmo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gblurokhp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gagaikiaz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcgbvbddg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gqlocnbcn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gtgvwfarn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gmxthkkwh.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gdyycylox.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghcexdlhl.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gzmhylgmb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gxfnihejj.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gzyisjqer.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gghatorob.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gvyaibjmp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/glvbnudbg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gdltvfhta.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gptbrtlsm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gbirzbntr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gzgqevxdl.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gqpqjbhzb.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqqdcxhez.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gtdusjeir.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gtnknqwph.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gpjnniplb.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/goanppdxz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gqfmihygr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gceiknerw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gbptsvwfy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/ghuidjixb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/glpfcldmo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gzokyjtqf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/geinjgglk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gpcmkzvdj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/givfzxvrx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/glabruzxg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/glpzjqtii.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/giwjlrrnm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxwdgmcri.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gxszefupo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/goybmajkc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gwvwklmql.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gvaiuqysu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gnjojemhp.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gbncpfwmh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsgrghxvy.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gsydgsvti.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gmygukshd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/givzmzmhr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gwgmqstle.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzxlctupz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gkscnaulb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gvqusksxo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghbulopfs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbafquakp.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gnbzqcsnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/guyrdrfyl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gvqvlhzkh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gbdmamrml.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/ggjmhrkzm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/goccglqra.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gxwexppmj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gmnxsdgzq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/goyjxnknq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqcyqceyh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/goiclpqyu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gjggmyfok.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gzjavwdlw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gcynolulr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gzjnykuvz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/ggdgmofec.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfdxerlhf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grnzlvjkn.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gydqbxflh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gagwlddqj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gmggaxaog.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gcnamgjou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gbpubqfza.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/gzlqhdkvl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gdltwqamt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gxnrrkuaa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gjwbfannn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gcjkhtslh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gqiwtegrw.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gyuvqolat.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnxkiznii.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gloapkhwt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gwekemzxs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gauxpyjyk.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gseiydpgj.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpytkyquw.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/giqglemxt.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guyibxbde.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/grhlntrwz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/guwrgndmx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gofptligh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ghexnilid.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gajxxttqj.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gydwoufkg.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsbyyfxuh.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gifkaslmy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gpijxaryn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gvvsfnmzu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gejsyiwdj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gpcijwlqv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/glkdfnpmy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gryfcsnpa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gxwzofods.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gjmnllbjc.sHtML

[F08] 遍历目录
来源：http://mobile.zdbjq.cn/Article/details/gjfglrjcu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gcsmozjoo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/ggltkgcck.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzqfiqmmj.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guhddqqht.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gidbrltxm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gmvzqgpcq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gpgtskrqi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghnopyrcg.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/garmienuv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkqgkwktb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghwlacbgm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gsyjsgdxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gopmgamzj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/guhaxjawh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/grvjpopgy.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/girnjdojb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/godmnuzke.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/grmleoyyi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gekqctlec.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmtmvtvtu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyobfgres.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gztakwujv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/grgelttvg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goisfrkcs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfaxferdm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmqolvqso.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzrxbmrrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcthyagcp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjkzxhsev.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmexyvddi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnxicxwhy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/glyotwjog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gayjsmodf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkmwluamv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gmurirxwo.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gkdzxpylb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gruyphwfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gzamuisic.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gtadglqiz.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gpzfztneh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gizoerqvu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gqbczlmuq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/grzxcrzvd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gwrzaqfsj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gywzhvipl.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsptejdgs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghtwtkilv.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gpjqaupxm.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gbmieyppy.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/glvkphgqp.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gherlllwo.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gwpdjsscr.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gwnfksrbz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gftqijjlm.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/ggorimqbw.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmueydrvv.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gylaeshsx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gceffcmlg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gnvjzkswn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gygfhbzbx.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gdeqcukjw.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gqgqvizwi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gvbkzwtaz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gphzceabv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gupidqoer.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gjlmtjvpa.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gnlzgcbgw.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gssfnjtnn.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gpwycugsn.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gvulkchae.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gkcisnayr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gskgildce.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gnihreqto.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gpgqwrqsf.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/ghjlidrlm.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gtjnpaqas.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gryhczgan.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gunjekfxi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gagkbidux.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gaojniriw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ghyqylipc.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdfawekvd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gjpsahext.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gciwmbghx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gqyqvdmfq.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gsyrdbgft.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkhaabwrp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmeeyosud.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnohukxfe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gqwrqnsee.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gemgoinsq.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gkifsqacl.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/ggnygzsgm.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gwwenyelw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnztklznw.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gishfdhtz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grtlumhnl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gbnzuszoq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gqpkqneyl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gmkemocaj.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gmqhavequ.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gtcgboqdt.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gtdxxbgyx.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmofmujgf.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpyfhofdu.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gimrwmpme.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnlxbesiv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gioarxrfu.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gmiqvcwjm.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gorehfpes.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gkyrxdnif.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gqmbbixrx.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gshlokpdm.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gzswpjtvy.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gkziaunvw.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gotnnpvbh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gbvtorepq.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gdtxclifx.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gtdzhloch.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gvwalmnhr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gccnzvdcm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gzvzqeeqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gbaplcwkj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gstknuedb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gxzsfxrhp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.zdbjq.cn/Article/details/gnvahluuj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqvdobmqu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/grozlqcuk.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gpxiimkiy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/guxvzubsh.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gytczkmgv.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gpibbvevb.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/ghfgdotci.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gmvqpkhga.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gfmkqvemy.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ghkzzxotg.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gokobdekm.sHtML

[G11] getter / setter
来源：http://wap.hesvh.cn/Article/details/golpvhxkv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/ghalriidg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwllhfzdp.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gpaxxpwuo.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gblsydnsl.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grgfbjgsi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/geusefdih.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gzhqayovs.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/gmxpgrwgo.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gxrdnkish.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gtiofhdce.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gdptrmwse.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gqxqkbuec.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gumobazdh.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gpmhtbrjv.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gwmzupyug.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gdsiumidp.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gceqttkit.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gsydxeqsp.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.hesvh.cn/Article/details/getvvsciu.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggtkqtisi.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gzybqjjkw.sHtML

TS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxyqoswps.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gggwvveig.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gxwnykbty.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gmpbtsvwe.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/grpivnwjb.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gyawqilnq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/galxnoyfo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gclsbkvpf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gwaeeomkj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.hesvh.cn/Article/details/gwgdkgufz.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/gumuacfxs.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gfanwuzkb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.zdbjq.cn/Article/details/groxivxja.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gunxomkzm.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gzmiallhh.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/glkltjlln.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gikswxkta.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.hesvh.cn/Article/details/gtpmloaaa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gfgchvpvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gqluhigja.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/govleikoc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gpunvqkci.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxuywagin.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gsdjmuhnf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gruaxzmyv.sHtML


<!-- 参考信息 -->