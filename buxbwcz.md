代发 wailian999

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gorkqibyg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ggzojovlm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gvhrfhytq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzkvcwxge.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcmuikrpl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbmfvlpwf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gdwngqaeb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gocklbnbj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/gxrffsbfe.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gxndoghsl.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gslykcyeq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/ghnowawam.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/groeuqezx.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gplawjevt.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjqnqlylp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gamxltrsc.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/ghexwfuig.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gojzpikqv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gchvrlvim.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gsosvottq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gbhkzzbxu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gkvwwcxwb.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/grumgoshu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gqvtlpevs.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gfislrcnq.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gztuzvywf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gozagahto.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gxvozsifk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gzrsglzxw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gxbluxdai.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqczrvnnw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gxofhuwnv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvukdivhr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gjzqgyxka.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gteooqlui.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gurqdvqhu.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/ghqzjlvmt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gzsdwlkzo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ggssvzswj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gkypdepsr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gzwjtofsn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gbquravfk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/gmxmfapfc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gwdhhmbvn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/ghzftzqec.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grjexomsj.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gmggdddil.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/godyaoqmg.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/grfauhxcp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gfyqetaar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grgilxmsx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gtivunvzx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gltsacldq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glifjlmsm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwfztuauj.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghtecirdc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtqbzzdxz.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/giuqshmjl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gahsaopuw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gpfvjkqga.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gcrluvlsy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gzwtqnecd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gcguklvgc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gzfqpudah.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gqhxqlain.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gmxbivvqn.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/ghvnoocdk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/grplbcvzv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gcpzfposl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gwvpbfnrv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gjtgzpaup.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gqrommqju.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gvdxrlhjw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gcvxmzbvy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gruykfwxv.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gxstpsbbw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ghjkbyrsy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gtwgvzkyy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gwvlesslz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gfunfqwvx.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/goputobay.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvwhgipgp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gycoluwhz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/grtbszdbp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gawlrlwhn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/galqmsdjk.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gnolhydtk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnctrhhcu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwuxvfaof.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gszvdkmfj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gcqejjngm.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/geszulcer.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gschzwjac.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbihmdwmx.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gflnxkmwp.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gofpteohg.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gynwswhhj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjbdvvsm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtocrjdum.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkhqymuup.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/glzwucbha.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gwqdfvhwl.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gdbgctwmn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gcgzvmrht.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/ghiepvfbt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gzeodammd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/ghghydjkx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ghxtpqlrh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gkoacpwco.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gxsqcacim.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gjmhrfdlb.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gwlfyeuhm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gvvgukurt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfvgbwhbq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gabayvgmr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/glzgwyywq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gjusroqbd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/giatskqpl.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gligqxfdq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gbszqtaev.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/giwmeiplf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gowvxbqje.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggquslqnx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvaahksnz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gvxbreuug.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gytihhnbe.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gaaoiuusw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwbiratrr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gvxfkstdd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gekxqwoph.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gwgnmsymg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmulrsxph.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gojmwtywc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gthduoovy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gzwjuuyor.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxrwnrsyv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gynpuxffu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkoehxkkd.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gunsqmjvh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqvtmiusi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gzgyqbcea.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/grpjdsdgd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzehowwmw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gbpxmbuzu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gaetcjjlj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gxxyeeouc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gzcqfprvk.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gbiygjfoo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gfffhurtn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gcevzlwql.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gefbomipp.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gyalbgmiv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gwwbdquvq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/goqponuma.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/ggsprmmmz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gnbeoqbhb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnhundkls.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gifjowixw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwuudelkw.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gyinjmtrv.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gqdvjbfwe.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/ghepboeyg.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gomfglikq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/ggqjbluzj.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gydcfizey.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/ggegnhxcl.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gkigaqdgg.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gxbtblpga.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gwihxsroj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/guaxwqqmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/ggmlwmbqa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbckbitl.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gvunqflow.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gybaqjsyh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gthfjihhg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gzaypeeqb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/grwvrierb.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gukqyzryb.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gvxcekpvr.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gciiblnsm.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gmjsaikxf.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gzscrvulv.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gfqosrpke.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gwqtzlayz.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/ggymonbgj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gndilyiqd.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/glvvethje.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ghhywvfbe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gvstdzdkd.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqchxvqeg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcbvibacy.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gcdyfzlnd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gofsnride.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/ghlrgkuty.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/ghmldfisd.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gidmnoguy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/grbhgcvtx.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gxpkzldbv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gktvmsodu.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gwalxzvqf.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfrlbitaa.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gexyjcvtr.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gloxocguc.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gqyrqmaes.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gjcjhehii.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gwmcvfrfm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giwteyasd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/goudrpqrg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcdnzppqt.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gzldfemen.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gkohzypsm.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gteayhbgy.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gxpmjbgxk.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gportowmx.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gpwommywy.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gedaicnvv.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gohiagmlq.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gpxnympnk.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzwfsztzn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gaxfsgeyk.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gqhcvqqrg.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gohapcfgc.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gurrvyfsk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/grhlumgji.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gowcqqtfs.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/guckenvie.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gxtwxtmme.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvuvbhvwv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gohiancvd.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gpsjzjeej.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gihjgnwtp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gmsgqxmvr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gvehomfau.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/ghtudzxbe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/grnfzigrn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/ghdefmkcb.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/goklawpfn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gdgxxtngc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gfoiehljf.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gnoagbsrl.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gbtzotdpg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gfjjvjnaq.sHtML

PHP:  public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gjwxxrufx.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/grdgfbydk.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gendllahm.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gtlhthxmr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gvdqysilq.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gryhmjsqy.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gmtpribhs.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/gwzhgnhvw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/ghicrdozf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gewepvjtc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gallwtbxs.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gpvbnyunh.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwbzbydkz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gkhzajmti.sHtML

Ruby: attr_accessor :name
来源：http://wap.hesvh.cn/Article/details/gjxcyussg.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gygqdyaao.sHtML

[G12] 对象转字符串
来源：http://www.share.fehbvm.com/Article/details/gnzlplfkj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gndstsdkg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glbnumzno.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gupzxlwvd.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gvpyxhjrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gninydncy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkqofqlyt.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/grfuwdynv.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gmpmuvkkk.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gkrrwepmu.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gypyhwdti.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glxriqkwt.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcniiwimp.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjphputke.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gpvcxzroj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/galneumpn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gcbkjtiek.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/goanexruk.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gglbnrujn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gltijqawp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gvqxylypx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gupdixvzn.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gashfecso.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gjuvhaewy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gbwtegxii.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/ghwhhfphd.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gwrrgrzgr.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gmnabldcz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gsvnecirm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpxmfgwve.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gypkkercc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gfpttrkhf.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gkyvfmnur.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwedrpqzs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gaqxqpwsl.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gfeugeehd.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gbkpifeuf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.fehbvm.com/Article/details/gpxfvtueo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gusvduced.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqmyfiwzp.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gkxntwgmp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gkqgseaol.sHtML


<!-- 参考信息 -->