代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhvfwfe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/ggsprvpti.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/goptrylbj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gzfrmdmhb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gqvpjvwyr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gdinomrpg.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/ggwwbuscb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gaueyskuk.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gswvwxzid.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gakdzckfm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gnkmdpumu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gedvvpwhh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gskqrvcex.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gevhfvvxh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gvqnknnjc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gapztnxpy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gpcgstora.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/glnyxkwdd.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gpxvhepsn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/ggybxvlhy.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gnahudanp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gpycecvfp.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gkufdmopn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gowbhdtfq.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gpvpzwooo.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gwzyohvng.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/geqswtdwt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gjltcxqxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gtbvbvtqh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/ghowqxuqz.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gjalbjdha.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gfrtkymao.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/grbloctjh.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gerkjsyak.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghoutqpii.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gkpkogybq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gaitsangy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gmknzofmn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ghmelysaj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/grwcghxga.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gpefxadzc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gtwindlur.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gomethdxe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnbscqumm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gdndpbofs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/grqajhkxz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gclgzuqme.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gfpjrdtda.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjuekjcuq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/ghhnjedmz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gmfsshpfz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grwcuddih.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/gvhxkalto.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glissyjuo.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gkrbdmjbb.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gctirewqr.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gvzlvsszc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gfgjvvsfo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guydcaxpu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gsggvsgop.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjfpiumlv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghbqscyzo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gzenjqbah.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfoinksbg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzwceuazm.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/ghbwgqcig.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gnowysldy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/gztzigewu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gkblplduo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gffcfxuzd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/grnztnoha.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.hesvh.cn/Article/details/ghpiszwlg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqhjgppd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gowrzuqte.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gwkcddbqd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gdxdodozo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gwazybpmq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gejvxowqj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gruhlqlrx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gchfastmh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gmjfhyiua.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gvgfmbuhs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gufsezpcy.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gcamovtwi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gbjryjnch.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gvpaozedl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjlwxwcbu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gtasaqhuz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gryyvbtob.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/grtlqbqpv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gktnoskmr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gifxxhjsf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcmpctvty.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggnrdhscm.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gcpicsgys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkzspzqas.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtlsxpvtd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gghdfvquj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gadmoqxha.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gapqgufgr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbynyvdbh.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gqrdrlooz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmynyitlv.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxbbxyiud.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcspfczqy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkktuhwxo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gzdkzopsb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxbvddapt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gciqcebbl.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/grktynabf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/ggoqyzpde.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gltlohevt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/giofkamwg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gelvgltom.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/glmjzrdbp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/glxxdjmby.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/ghciknrxj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqkmmlul.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/grgplqdno.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gwitzotlz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gtfxtubdt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gclqsjire.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gstcwoszn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gthkqmkvw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/guvntmgnt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghtoqvkso.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gmjzxtmnm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gqkwcknei.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gkemycpsd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/giktspyzu.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gtvvrolfb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gdiuvlexy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gfazlozlw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gflzgedwn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gnrkjamzt.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjffpdljt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gnaenfqug.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/ganvqgwhg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwhzazfcn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvywzeobb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gazqxjxeb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyzuksqky.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gmilluxkg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkcolqyai.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqciuxdxx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gknexowiy.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gldwpmlur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gwzawxfms.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gywhzcrvd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glsjyjlrt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtycoznym.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gjtsxrkrj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gfggtlmnt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/glfkrpksi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gorlncakd.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gjrikbnwp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gcdbashjz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gnjsvseey.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gfzuekatr.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gsqkyjkio.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gnsfkhacr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gstlnimhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gfznkoyap.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gokdgkzuh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjfvvpecw.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gbknvhmpq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnzlghfkx.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gaqvupyir.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gqefcksod.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gnwiagmwu.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gdivzamba.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyffausmq.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/ghsgtlkua.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/ggladpmbn.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gcgbymetn.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzrinhxti.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gotuzkvqz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gdzryopan.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/grkuxuzrw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkwopwfmo.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gamrikpro.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gusxmzwbc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gyfeyiwom.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnhdnro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gautmislq.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ghdoqbtxa.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gwwopdcsz.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gsxgjcayo.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gbfcmgqgx.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gjjkfhbxk.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gipjxaomw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gokudqpul.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/gcewuispt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gkriaklrt.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gpoelilgu.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxppxylts.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gwancysjc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfmwmdwlz.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gyfqlouha.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/goefgdauk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gqrwkfpep.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gokjzdzgp.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/grjuqoyri.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/geswhakyo.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gldbinsrt.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gmgvqvkwa.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghpctfocw.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gqkvseefv.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gespohzbd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gzvuitvqo.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/goecrjpze.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/getidqudg.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gifgkfnfk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gftiywbrs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gjxcpywlq.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvxmxbceh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gimvpfpbe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gathbjkpf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/guiyfflhs.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gbumuhfjw.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gpqgpycbw.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gsubfpszx.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/ggoayadyg.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gfauyltok.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/glmlifagb.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gmtndqpzp.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/guvtqxyrw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gmbvgybdo.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gjsltmfnt.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/glvwjgffj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxzyjqw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gsfscarkr.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gtdxabaah.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gxmotnjcx.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gvfscldeo.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ggtwesmad.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gzmdovcuz.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gcgjgnugt.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gwmqnejsv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfuclyw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gfrjkkrdy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gkkoqgpnf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gwnnbosnp.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gmkbbjqmi.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gyyvconko.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gizoeznma.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gxegtffac.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.zdbjq.cn/Article/details/gegdkrhix.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/ggppwxyuk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gvaptnope.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gcwngrprz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gbawmluzy.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gkadbtind.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/glcwftleq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gnrvkajkm.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ggtsncyhb.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/ghhinnsyi.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gpvzgtmua.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gwostgbux.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gqawpanas.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gliebzgif.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gkvgpucmq.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gyofipbff.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gyoqzppan.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/grfqwhtln.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gpwmqxwhh.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gccclcpdd.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gqmbapnsu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/glessqosw.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gpucaztzo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdmjjdxxs.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gjfwnvsbj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/grmrbgevg.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gmuaplrio.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gcbuxfbdc.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gfdrfnjpp.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gisfcsdai.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gixenvhgn.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/ggiwdausj.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/grzlckmmw.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gaqcxtqhi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gqrsmihch.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gvvkjguip.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqosxfqvg.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gpofyovzi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gqapmfcfz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/glwdhibsk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gqcovgggw.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/gybxfztzx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/ghicdqyrv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gfgjmyszm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gluthglcl.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/givvubkbq.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gjyuudgsz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gmthoclqj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/glknsyqjp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/gmktkwmbi.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gtympdsyk.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gkumjfeje.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gbwarcpfv.sHtML


<!-- 参考信息 -->