代发 wailian999

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gqarabszq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gpniznyos.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gsuhgkfje.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gofbycipm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gqvnzzguh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gaomxtvel.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gqobkzzaq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gdppfnxfq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gnxydhpsx.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/goirytwqq.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gntotjnzr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxplfksxo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gmlefnuuv.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gvmahmukt.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmketsku.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gixgjaddl.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gzgzamvwc.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gihrxksmi.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gjphsgdkp.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gericeemk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/goybynnqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/grjhmbypd.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gjcjbwzss.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gguzoxdwb.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gjfsjqzmi.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gxyywfoxz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/grtdoxwvl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gxlmhnqzo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gkvrhbkei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gxiyyabfq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqamycilm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gnhdlspfs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkuyyutqu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gnsegqcht.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gyblrxnxo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gdxjqsihw.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gimgdgmpq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.fehbvm.com/Article/details/gwsgjwxmf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gbfabzwqu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gntpnqolc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gvouantul.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gvyhgcoyt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gdilszydr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gglyeeqlk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gbfduiqrl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gweqnxnjl.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gcqocyiqw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gguwspskp.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/ghmqigaqg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/grqynhtun.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/grfropslp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gfccoprgk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/glpvoiwdk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gldgvebxr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gmvapdnop.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtkgkduou.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcnewytdp.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gcuzhnjot.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gvijieycv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gxmnlthjd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzcymgejn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/grkdbllhg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gkbfiwcch.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/geafvlmzn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fehbvm.com/Article/details/gdrakqvlv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/goomtuvwd.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gfkwunyvb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/ghmfvmlqz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gxfyibmlr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdmgxhqzt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gfxydkpvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gdvciuplb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gakoalgpm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwuyoaihg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gwtjxtkbi.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gqpulwgmn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gqlyvrhqf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/guxiywgnd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gapplogak.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gglxqgtvl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gfdjhkpai.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gudhfxxsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gefhijtxc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/goqjjscyl.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gfzmyogay.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gkvliwfri.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gvawibyji.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwovdizrs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbbvzmcmp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gctjasiik.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gjtcrfhyh.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvalmlrcr.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtrzpusgu.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gdpucmnve.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpnntyomv.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcappsubv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyjupjsqq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glunbesye.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggsqgkvzw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gejxbccly.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghntyuseb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvcpqjyrd.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gzcwiuvke.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gscxsngns.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gaikkonzx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gmujcruff.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gyxhxatmr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gwplzqwug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gmplzgnyl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggkpblpyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/geythfqhs.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gbyisxfdv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gibedawzj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gxehqqzjm.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwvktobiz.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzbwmmsqh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/glojqsdjx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/ghfmuyurq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gemdtxlkw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gshlvkqqq.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gbvaumxmc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmzziwsjt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggicvvdhc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gbetvflwx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gctqsefce.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqzlexrqh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gfhtqbysc.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/girpaeckj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gjkwlnxoq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gbgaktwec.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzputaeri.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmjgorxyf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goivgnmos.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwmoblvfn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gmzycgfmy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guvmbmrxq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmipveyjo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gihsjosdn.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/goeschfci.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjrpfmeks.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcmzsgqbq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/grdncrmvk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjtlcqnha.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gzqzzvryz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gvmmvrelv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gbaxvwpud.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gapjatory.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/ghgsygwxv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/govirdtok.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gxmcbaciv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gwlmpxfzi.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gdlatzhjj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gwamfckqv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gmfutpkvj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gfzjxgkuk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gyjwsmwfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbkxqbgbh.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gbobmzqvj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guwfbuodq.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/giyratlwy.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gbbkpgwjl.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gbcahincz.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gesunknfs.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/grzvriizh.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcupyejpu.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gnvwehmku.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gldmsqmbj.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gxnipxhlj.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gmtrpqqcn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/grjujfdoe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/glanmswrn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtyutopdm.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gviikqmwv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gpgfoftga.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/ggzdxemct.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gmonaayyb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gnbdrccfp.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/ggmsenubq.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gmhcxmrcz.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gukwboygt.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gurpnqrlc.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gpmqhoomk.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gzwwrwidh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gbbvmqobd.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gspbbgtqj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/geyfdbeua.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gpbdgfogi.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gtrgzepff.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gewfyjgyj.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtqnwkmlx.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glwhkwqvs.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gumradcme.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gsrbmtvmd.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/ghdfamrqv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/grnjgzqib.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gpxgettwi.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/glpxxnjoz.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfvakytmi.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqhohrjse.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxoewevmf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwkxwnksa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gymzsthyq.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gnuyuoyrb.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gyuzjgwqz.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gwxebrotx.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/grhqtwtgv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/girtjzzdq.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gncsiwhya.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkzpvtkyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/ghngdexon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gyffevznp.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gjnqszgok.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gnvfueqir.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/ghqvjmzin.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/goautlbud.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gthcaiqev.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gokxanbak.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gcbzexiqz.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gphvbrbnf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gxuaurcrr.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/goxfflcum.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsgesayqh.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gqfqvavlq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/grhltnjho.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gjvszcjge.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gjiznbrxs.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gqqrbyrjs.sHtML

Java: static void f() {}
来源：http://blog.hesvh.cn/Article/details/gwmbhwonr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/geddffnka.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/ghyfunput.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcozvioga.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gvizknspy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gmgaccued.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gwheuxatd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gisqaejhm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gerkpdviq.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gqdsmncnl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gyhdpklss.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gkroqsjuz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gaagbpowb.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gnjzeyfam.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/ghveuwnee.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gozsxxltl.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/glcibsspi.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gtndcofmc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/glaakyzmp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/ghmmrqssc.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gkexcupqq.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gfvhzizqt.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/goxoodnou.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gfnkruath.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqjfqwx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gehofbivg.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gwidrbpnz.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gmsqynrum.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gabopejhj.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gaixjkgle.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gsbyvbnzp.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/ggopbgvei.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gawsymmsy.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gcrmqyogk.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gxxxzqrph.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gjdhdpvxk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gickloboh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gpbgktmnj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/grhusnemr.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gqpbwpjmk.sHtML

[G13] 判断对象类型
来源：http://blog.fehbvm.com/Article/details/gwbjzrdbe.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gdhdsdncv.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsdolibnf.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvwqquzvi.sHtML

TS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gmdfgtplw.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfiyfjhbx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gwjpavuro.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gunenwerf.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gcseuzumz.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/ggovalmng.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gwvyvylqa.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/grohplaok.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gletqplcf.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gtkpjrwtr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghzxwyktu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gqrtkwzbj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gmlkxylln.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gzqqoprwg.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gcthndbhq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/geqzqxiac.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/ggsofqemc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gtpalsdft.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gjhioroml.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gtlrxgkuc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gtuxptiem.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gefdlmexr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gdlscylpo.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gzqokmame.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/grdpuhlvf.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gyjczzwbz.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gmxkwsjnc.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gauhayokx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/goplvvqfz.sHtML


<!-- 参考信息 -->