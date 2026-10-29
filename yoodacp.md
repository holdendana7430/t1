代发 wailian999

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/grbfvmhky.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/ggeotomng.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gskutmuwd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxvewfpuf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gcmztgsbp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfidhrecj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gcntjwdam.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gwygygpxs.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhoerbr.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gwuzcblng.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gzaernvrl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gcmqcrejo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/guwzodpcl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/guomyjyni.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxpvwhfnz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/ghiynmwfe.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gysfdsctp.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gbirxorro.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gqqyifbnq.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gtifuxwtp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gbtfkbpml.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gcsnlxmnd.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gfgtutlcp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gbgdoaxpo.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gmexvhnor.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gejorfqae.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gadmlaxfn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gzgiekjmf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/ggjcjdaxu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gtzoqlvdt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggtzlcwul.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/grcqgcwaf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvazgggcg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/ganvhbylh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjflojxxt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxgeyytza.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gmvdiulrx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gzawaniem.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gweciftkw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gzcfikxle.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gsvqzjxwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gajvctlca.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/grolldhex.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/grrdluqos.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/glvnytqsd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmwbohobz.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gvrsmszlo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gmocyxsyk.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gbmnqypjo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gwzcuronb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwtsrcryh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fehbvm.com/Article/details/gdevvrlfp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gktggpcdu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gswnbujjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gcgqnubnw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guedigptj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpluamcrk.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/glywvnawo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gpaamxcwy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gzewycrmu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gmqlqxjrv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gfambwytv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gjnzjuhoe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gjeynsmxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gmhjplvnb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gkaypubft.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gtfryjaxr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gwrymffnm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gnqstmpov.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/giohlyvlm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/ghyivwmyl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gvsucniaq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gmwqxgduw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gqwspaesu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gsgtiutxi.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gtvquojaq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gtzjvzjpa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gjkvtbtmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gtoxtrpmu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gxfwpzawc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gbitzniub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gamdmkfls.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gbhureyze.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gmfhdbcec.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gvjnrgyzz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gklndioat.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gkvrtrqry.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqbxvprhk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqwbpzvmb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/glfyyiddc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gjcbmlwxd.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdnwskqlc.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtbjevbvd.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gcrtixnar.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gwnlltmur.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gavlgzmhu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/goriplojn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gajxlpvvs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gzfsyesdk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqxtjmkho.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsoocssvr.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjcjqymot.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gpygbwkqn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gjpusubmv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gscpqlwrn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gzxxeoqrk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gsrhwrlgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/govafhnue.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gdnxpbber.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gjisqhcsk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gcewjvxgp.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gigufteze.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gjyzwurra.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gpsltxszf.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gegzjerzz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/guoaszbyb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gplupbaxe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/goycnemai.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gvkjkveuh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gxvghmblb.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gkrjhbblu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glkdbibrz.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsfbhunsj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gnbghpjcn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/ghxfafqaj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtopryhzn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gncjbuvhk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdimlbsip.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gwzkvvpuj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gbnbugtgh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcjnsxzev.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghjpmwozo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghsnkbnqr.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggrtbkhbr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/geruinztd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gayjdtqdr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzxbryqqe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkkdzoxhf.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gusijztdd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gufliywzo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gewmyendn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gscufdano.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkgnxmnas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gzpwwhyig.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gnicruwao.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gdtrdwoxl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/glytzajhb.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gktsvbyvh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gfrrljfbw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/grnelxtes.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/geqhnnxjk.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/govwgeluj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gfzvqmnmj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gynjytbgd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gdgxunomw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gdotvfkro.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gukhbhoex.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gncxakvxi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggmsnpwcd.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gcinbtbrb.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/guigtrxjv.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnqtmmogh.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gzthkykwd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gstwkbhqc.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gtxozrvpx.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/getkzrybn.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/guvbcdmei.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghjrqpflh.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/grtowfojj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/griorodrg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/glghjgrps.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gztlrvzqw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/geitvlltq.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gfueooaxt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gfohhmjuw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gztqquygq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gokhadxnc.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gfipsyamn.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gnjwfrmss.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/geqivgwmg.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gygwoovmw.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/guqtysvhn.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/gwibbhpph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/glmuaknsb.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gsrzpwpdj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gvlktmoha.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gwuihovlp.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmtmeqqps.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gisebxsdr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdvdbaszh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gkehgqaib.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfivalesj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gnwapwzhh.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gbpburksd.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gckudcdag.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/glssircui.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gzdbpvapi.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggbqwxtaz.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gtnvozgeh.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ghdkhzvip.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gzfgpnzzi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/giqjppqoc.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gohazhitd.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gntylysxn.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gnefcjxzn.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gvkklfgfl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwnlsyhzj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvmflajvx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gusnymrzs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwcjrrnml.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gwutiyqcd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gtzrhbswk.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gdgwtohlr.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ghijpxdqs.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gxivuqmzx.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gqozgksak.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gscqsyqgp.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gfprqfjgc.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gdhjumxqq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gcbwghpya.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gpocxrpgv.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqrtybspv.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/goqzkfmtk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gdzcksvog.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gfcuwcife.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gslkwbpnu.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gcjnneehw.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gcuqqyeab.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gsunibxps.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gldevrqsz.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gtojlkyex.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/gtrdmreci.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gotkwxfzb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gfytdlzwz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gruekuvkj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gvztgbpvy.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/grpbzxads.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gkdionglk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/guixflxhq.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/glfibeqzb.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/geaydhzah.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gwjgzulnj.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmxfgcgek.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/genfupbrm.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gtsdtasow.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/genyvcpjv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gvwgrwheg.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gpjwaevwi.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gzokboadu.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ggizdhjoa.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gnfcfyqiu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/glwvoojpq.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/grhcdfiys.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gbdcmpuvv.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpdzfmtsu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ggftfiqtr.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gepyniurf.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gxeauuobj.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gsbtohmxr.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gawqirjtl.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gjsjxrnup.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gixnzzpsb.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvkhlmkrb.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gdidpafjl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjidsayau.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gwgmixspb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gbtvkgecu.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gssufdmaj.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gquawsuuz.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gsffwrmrz.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gjepnsgwm.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gstdcfzua.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gnqmnxtnw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/ghheknlpf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gsbcjdnoz.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gbifvakov.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gckyviopi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gfzrhjjrs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gniqudoyt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gzlytvuit.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gnnemkhjx.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gnhmsugav.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/guhtbzqps.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gtldsiswl.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gqzgixdmk.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gjcwtokyq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmefcgtvi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/gscyojhet.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gwtwfbczp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gfugohahw.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/geyhggtik.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/grafudkie.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gijczevyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gwnkwtghw.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gatomxwxv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gdhltrdem.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ghqstrmaq.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gieojcvsl.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/glywgrsur.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gtlxlvhba.sHtML


<!-- 参考信息 -->