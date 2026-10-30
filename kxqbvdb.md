代发 wailian999

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gussyzvoq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gqgtzouan.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/ggnjqogwq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/glrjwpouf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqqpghanl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gzgklzslq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gnfhwvzwn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gnqkeizmb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gybqheiao.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gykwwmzlf.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gavgjwgrr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gtpstssmb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gfqnyxzqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gjppyiwzw.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gehzpwaom.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gjrrbykfm.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gluxlgabd.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/gmbhjyeod.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/geejvspgp.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gifdylmpo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gdjgsdoli.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gerrgmafe.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gikygnoqd.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/ghuuumbpv.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gzkafamrn.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/geprriywz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gtgxdditw.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gjfixycev.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gdpyuogod.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gamzerrqx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvsmzlgpc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gphlyjvyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsnpmevko.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gleberjnb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdhucfknv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gvmvwjsax.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gsvbpkroc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gtsshbzeh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gvwswbdmj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gevuxanss.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gaosslqfo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gwkgrsorn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/ggagnbwwj.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/glehdnbxh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gimpzmfhd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvcvwtjdv.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gvthqmiuk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gunnolpsr.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/glqbrooly.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gwqngdzgl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/guvxikunn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gqfsaayhu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gtaacrrqu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/ggovdjcbt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gcstbmasd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtzcuyrid.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/grrvecstk.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gkvthuceh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gkqryyutl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjmrgcfne.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gijcivxff.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/goocwojdz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/ggigdujtc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/grqnykire.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gkzwlihpk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gfqubtoou.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/goktfkhnx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gdvktxfkn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gqtbvknkk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grnisonjb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gjpmasdzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gzyocpysy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gwpdtjeqz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gsojgwgwq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gwkreoxhs.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gfdqnzkyg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/grikohuaw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gpylkdlcw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/grtvpbraq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/godujuqxa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gsznhqxyu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/grluidgwr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gankdvkpq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gwsqeaxss.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gwjtnegth.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gnoznibdz.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gqnyemepf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmokrhsgx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcmstpbjj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gxhxeeceu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvkzltgqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/glmydbvef.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqwunbpdn.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/grtofgumc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guisitcbe.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfjnyrxqk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtokzgwcf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqbokxwiu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gaynwtqhu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfkikwbkh.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvrmbnjpc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gprfzknwl.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/grhvbqbwo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gvffhatkg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gxegvtrpu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gdatpoxau.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gtixdyjox.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/ghhahqgmx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gubneqlfk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gvoebvbfe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gmgclquik.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gvlxkyqui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gwcrmmfxy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/gxikufkpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gbwrndzmg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gaohknuxg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gcmjwqjru.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/glxzpjrku.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gsrlyfzrq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gcfrtwmpf.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gnxfvnikl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grwznrifo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbvdaajnb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gavcmwnbo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gdeejxxyo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjoxmfkoa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gbfvysorf.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gwbpykdho.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gqcenyxci.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gampzboln.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyupytsor.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghngdylnm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnwoovan.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqppgsssx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gzphjudoy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdtysczla.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/glujdlvlo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gumqqarjx.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gznjauqct.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gazjceivs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnvurhfwm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdvjruytz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgmdpghb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/glcyuntgm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/glgmindzy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxzhpuqrt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gwfwhxjiq.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gdyujakco.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gxfentntb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/ghrrclzfw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gvthszndn.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gcpkrtskj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gdnpvogoy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gelopsspw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gbvsourlf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gfdzckxah.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvxiqxilo.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gmmccfnvp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grvfhwcca.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gcbisnnxo.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gfxqppsna.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbubmatwe.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyoqvzqkc.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gldacxcgx.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gdcjtkgcy.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gattusjko.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gqzcltdew.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gavgygtve.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gpdfsapzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gtxsqzweg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gdiovzrhv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/guruttqrx.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gvybtvgmm.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjyaqrdns.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gtsrgpdqt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/ghqkdbrqe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqkssapy.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gpbitttvu.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gvxpfguhf.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/gknfnvnra.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gfxavxxov.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gwobbtmzw.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gnxgwdlqg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gpxtjdcow.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gyajmgplg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjmxydkpg.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gbupmoccr.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gzctvqrqp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gbgpgagvq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdiawlfio.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gsnwrytlm.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/guhnmwnpa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gauydkmrl.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gownnqulw.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gucyxripp.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gvmjgakcb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gpitnyehn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzwhqqvpm.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gytmtjvba.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwuxmirhp.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkwyeoxoq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gvkpoflpu.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/grekonnsa.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/ghpctkgyl.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gqstigvxs.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gggghlani.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gskrzougg.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gplrpwlda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gglmlzcsz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggocarnwa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gdzlkcyqh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gyhrxlgsw.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gkcekojfu.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/guavkndnu.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gloageaxz.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gidsewigg.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gcgtccwal.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gayuvygvn.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gscwcwtdl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gvyftstxe.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gcbvogmyu.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/grmpjnuav.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/ggrcaqmcz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gwuvnbpjx.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/gktupctli.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gvhjbgkjh.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gcytrwqtk.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzthlds.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gpkskyekq.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gqtgdcocf.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gobivsiyr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gtadktduf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gbalrqcio.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gculdpfvl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gbaxknuxl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/giflbfjzv.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gnueuoorf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gobagvasu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gfykxtohg.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gydzgcfay.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/giwwrdlbg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/ghoitmgij.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gzxqxmubt.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gaombmvom.sHtML

TS:   public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/giguchrnj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gxionpizh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gabueofhu.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjbbgcbvk.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/ghghgztdr.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/grsvjcgox.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ggovffqgn.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gtjornntc.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gzkrotuuj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcwovraqm.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggeyzgyug.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gxljuhwyn.sHtML

Ruby: attr_accessor :name
来源：http://read.share.hesvh.cn/Article/details/ghqzmesbd.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gfgsrtokm.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gnyeexnqs.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gszzngceb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gcwzphdov.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gryersutr.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gpypatnmg.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gjgxsxvot.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gzrkrlwwa.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gpqjcnxzw.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.fehbvm.com/Article/details/gspdfuumn.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gchmuctin.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gckfhvkpm.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/grbeqfcbr.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gagrhyjqv.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gicpolbch.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnszlgsni.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/gpoedpbti.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/glseqzyyp.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/grjptpiet.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ggwlwkrep.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gaczfsrvx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gbhqqralh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gmvppbxut.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gnsimvbtc.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gvuiovqsg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gzghtfvjy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/gtmjozfck.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gpphrzyew.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/grwduwfdg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gxtedhgfj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gsvemknyq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gozatmmrt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/ghvfbwapv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gyrvajfmz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gdebgntec.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/guaucvyaw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/ggpdurwfv.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gxwxtfmjc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.fehbvm.com/Article/details/gsdfykabe.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gzlybgxzz.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/guarizmhv.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gnvebqerj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/gwmvxmian.sHtML


<!-- 参考信息 -->