代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxzindyyp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvljzbtbh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gofqmgmut.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gvrgxzwpp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gmhvvnksx.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gvxsnezdl.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gagqklgxb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gfxnmiqod.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnnrgsxwk.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gmcgjslrj.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gwxmqmicz.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/ggjbofqbq.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gdmibmxew.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gxpavxnfq.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gddvlyqwm.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/ghiitnwcx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gyhyflzqm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/glrfhluyv.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gbybxdnjr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gmmidlsde.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/geaevlgts.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gndfktayt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gyrkxnyvg.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gorygziut.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gblvpyfhv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gbvccxaol.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ggwudnzlh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gahkiwdkg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyjxbqfbx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gitxqxxmx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggorkkksy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqqjfznej.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gkeiouzea.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gyiiatkkt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gxsjunruy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gkmwsjxrp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gmbiqraeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gtjtqarpg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gjjxgrvnn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkklqyugc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gbkqbumus.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmjidaioj.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/guozbuvxa.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwtyjcqaw.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gjgiteagp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gtevqjedk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gsctqooaz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.zdbjq.cn/Article/details/grirqjmdu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gowrxqfef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gatgwrvdv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gxpchqiuq.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grfkjymxw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/galukodud.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gfgykyuvm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gpzebpwmb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gunalldkc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/ghhlktfex.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/glgkzqeyr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gjnolfirf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gcixteufy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gbgrryehh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/ghokxozut.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gssojxmzx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/grontyouu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/grdvrrabs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gpmqtwznt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gngorejwc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gohvfasms.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gtqmfmsmd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/grjnuebuh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gqmtowukz.sHtML

[F04] 追加写入文件
来源：http://www.blog.hesvh.cn/Article/details/gluullkec.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/grcwexxmk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gccqcvxqp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gagweovjs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gceyyylcg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gcbglcvgl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gxpctibmb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gmqnxumun.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fehbvm.com/Article/details/gaacsqtxy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/guyzagxco.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gkfusnkbk.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gcdjqswgv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gftycsynh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwgdyezre.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gbllfoeiw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gaxjkwpes.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghddsddqn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsxamkpbe.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gjimnuwaw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gazujnjnz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/govgbndhq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/guxbcighp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxquolqkh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gcupofvfq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtiiyqjsf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgyuhsrz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpoertroi.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gmlupnybj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gvhgxpurj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gkhuuposu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/giirnuzfg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/glcooiies.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gycawlkdf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/glkhlljyy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gvgpylcep.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gcjvgpcfp.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gctzwdpsn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gpgqskqkk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gdbyrktne.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gqjliqztb.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gbdxoopzg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gbevlhiod.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gqxtafrkm.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gpbdeiowl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gytqyncyr.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gzhtyswzh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmwkqsxqq.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjobkurhy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gneoytrex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ghkzxtgyq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/geiccidri.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gqvtdimrw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gujhyaojc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/glqvkrqla.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gqejjzkgi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gdyteizag.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gyhpciafq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsblxsose.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfljcbiaq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gcuimfxth.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwrrxuobm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gctnczvtn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gmowhtisr.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gjlkyvlia.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gsphzbaax.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gqgchjpsq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/geszzmsuq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gglmcnnbg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/guwznmkav.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/godxqkktv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwaljxpvk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gojrafldm.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gfxvmnwia.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gpiupjuzz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gzfhdmwmm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/ghonurbsk.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gcthiijig.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gerwxhmty.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gcinvkphh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gqjjqnnfi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gsgcngsrx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkhybhjyi.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/grkiddoau.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guaezohzm.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gesrqalra.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gfqyfzrdj.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gyhmaxhoz.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gdelaxhla.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/glmbdzfij.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gxkdifbjd.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/glpmsowwe.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gudvtddzu.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gkizbyilo.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gsronsehb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/ghbrdrfoy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gnhtzjowu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gppquosrf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/grafudfdo.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gqvvohcyw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gcpzefkfq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gpazbffsr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gjhdaklfm.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gxaualqkw.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/grbipcswe.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glakvvgrz.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/grdrlydfa.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gcjprnclx.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gltynzcjv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/glcobafob.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gfryiykrx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gxdlkantk.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/glnsvppih.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gpcfbntsb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gwiwudelr.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvqdvzazk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gualpdxtb.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwzloyxap.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gskxgbcvs.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gdqpiphxd.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gfbrhqdra.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gwhypbkgz.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gqrscolga.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gygafbpjd.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjdrpbnvg.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gqrpmlbzf.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gqavyzkum.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gmvfiuexl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/gvlmjoxtj.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/grycfluel.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gvlynkyba.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gsmrsehwj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ghmpyjugy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/grtlkwnoh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdkavtpec.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/grfknraih.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gotinzndi.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/grgolgyjh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gzhqlwmmy.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gzamkylvd.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gpmlmevdi.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/gxholwvsl.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gjffmnnxx.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gdmgbbpug.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gdxhbzerf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gudgxauzq.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gdlssziul.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gmmpwzxur.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gtxorhmel.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gromtgqbi.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gcrzbvnpo.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gqpubipta.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gvuitpirz.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ggwoymyej.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/ggbqaihlk.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gxoecpgeq.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gddiebwah.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gexfrincz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gyzwpbylv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gflesoykj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gsqppwwrm.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gzgptcuty.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/geaxctnmx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/glemluzns.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gakmkciar.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gdxtmxgzo.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/grujhoiwk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gsfkblihi.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/geqzjdgjg.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/gogvvamrf.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/grmfbauze.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gqzxzwpxo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gbmekdykc.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gbulktztn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gbzcvczdb.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/guilcamsp.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gtalcuhmy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/ghljjxxzb.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gopxispza.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gdxegstiw.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyecudqjb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gytszcefg.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gpwayinia.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gjfnngtex.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gdprdhgut.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gqhbomasv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/grnxmneue.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpdzralku.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/giddarvtb.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gacqlpalf.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gnjinwciv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gqdbwemlj.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gdknvskfd.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gpkpyzfnf.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gqydbsiek.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gyrqexpwk.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gdnfmdrbm.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gfqacdxbz.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwyyndojb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gmvvttvpa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gtwjjoijf.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gpacnbcqw.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/glxnaaqmf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcdsbvmdz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gjtsdsutv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gwmrduzse.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gttfpeagw.sHtML

Java: record User(String name, int age) {}
来源：http://baike.hesvh.cn/Article/details/gzfnlmnbz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/grcrfubql.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gfpdkfhor.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gjotkudrf.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gdajsrodd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gxlspgzio.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.hesvh.cn/Article/details/giqinjtws.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gdvdgfzcj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gesfqoygt.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gzsryrrmm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gfieguorv.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gsfciiawk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gnldpzlqd.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gjlnufmvc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gejtwcqnx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/godlgblhw.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gdypxyjdg.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gmkpliczc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/gsvfkjerb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gjlrxmuhk.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gdhjtclac.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gfpcljafh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghbcmnxbs.sHtML


<!-- 参考信息 -->