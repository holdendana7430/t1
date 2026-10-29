代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gxnbrqliu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gbvipcbwr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gutdmnewc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gfzhuwtlq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gvnaulrfs.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gmoofwqmi.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gbzscutye.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwiqbeqli.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gkraifbxc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfknszlei.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/guofdjhpj.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gbtrdqwwl.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/grmvanfqd.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gvllllqqx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gsopuvwsz.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gfujcbaxm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gpmrhlauf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gjnixdrxb.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gcujasshn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gevqcmjls.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gxbrxwgwt.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gblahzyah.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gliarsgid.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gfpibwftw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gybhtegfr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gyouhubdc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqwyskzif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmdahjrvx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnainywvr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gazpsgugx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gruulfuat.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gezngdvxn.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/ghtuyqoqn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gewjwajdz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gngwgfbri.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/glkuzzjbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ggrkaselh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.zdbjq.cn/Article/details/givttatef.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gttuqedlb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gridggzth.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gtppexxzd.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxkfnskco.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gutqigsiu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxehoruth.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/glxthwkki.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gyssjkuck.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwekczbfj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gcjxyxbkq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gyqwxyncg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwkglojmn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gyoyiohus.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gorcupstd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtkjckfwg.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gswnaywyw.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gijqzurqr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gmvlmtjdj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gwrnlfuoc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjliztvgb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqnauraed.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gojkwpsrd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gkjqwlztx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gpwsbhfzc.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/glnkuubzs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/grzupaxzi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gynnzhljj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/goxbjvtep.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gwowcjhym.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gslfzuamy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gpjqcvzje.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gzbmsburc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gjjotdkpu.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmshkdynl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gsmtajqlr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gqtmkpyjd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/ghpvvwkks.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gmyqgtgme.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/grbnpqdeb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gbcvxmqdu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/guzuavvkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gyeglliez.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gqiwlvtye.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gajijugiu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gposxlicq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsxexztcx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gciwxzbem.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gtckfwjcx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gkudzgzsz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjifjnfia.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grgenmfmp.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gnyohtqtf.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjqzorgpw.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gexoaxdhl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaifobbxm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkeavzxwn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/guyrrtbna.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghxaiwnhb.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gawppbiwt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/geounfzgz.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/geqzchuqk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/guqdzdwhg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gujkagdny.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gfqsmlldu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gdncvgnhm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gbxbjwrnj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gqtpqymjo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gudfntsok.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gywgakiib.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gmwoevsrf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gbrrugban.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gttwrddyw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gsaqrmgpg.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gxjuxcaqw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggkhyhebs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/ghfhxuyfx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gificextn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/ggltdpfvn.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gucjiaxwg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/goguenjhn.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gisbuwtfs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gyognziqu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gybcgfeza.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gtfavrzcx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gdbefddwk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtfoachzh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gnvldtkzl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/ggsbfbpaj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghynoiofb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjhoysubw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ggxtnsthe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggdzbbbrt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/giankfvhj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbuycjfzc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtgaxmxov.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/grjffmhss.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/gfajoyxsq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gotdzaiit.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpnvhpanb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpduiyfnc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkaaeyncp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gcafgkvml.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gbmbxhhtv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gfnxgyzde.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gibnyjisx.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ghiopzuwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gpakijuxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.zdbjq.cn/Article/details/gasikcfxx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gmhfbhboh.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/graeldqfi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gvabuztnh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gdsotripn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gypmryetz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/guoytphlc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glupyxgbt.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gjwutzxfj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnmsbflyf.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gnnnzlvit.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gkglzoovz.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/grlbzobri.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gleguzriz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gtaeqpnjx.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gshzlkdey.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/glanqbipl.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gueodysbh.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcpmgrjjb.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gffbbauhp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gtfzdvzcl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gqcwkldpj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/glfyfzfod.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwkaqthom.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gbqacoptp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gwyjmuskm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gictbwmwq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtpidqzta.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gymnsncoj.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gplvhkrzf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gomzekdun.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gjlyjqxfg.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gfblnvizu.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gtvigbehg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gfwbacxfc.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gboowfyae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/grnwjtsjp.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gvskgxhxl.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gidalezbg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gyfhltirz.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grmlqflda.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gzlsqmbqr.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gzrkzygcm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gejrxufpp.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gmsaeuemd.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/guiijnqnt.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gbtedasgi.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/ggbhbotgy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gwveddgrv.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gbtxbxvkj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpqlkkice.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gxqxywlow.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gmiaxpzap.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gmblqcfab.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gluskaasa.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/geuavgxju.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gvnolqjlv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/grrfowkgt.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/ghmlnhvwd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmrcbysen.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcvgztsrj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/gntfapohl.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gcshleehh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gfgqqghey.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/ghpxljyvz.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gptyaoegv.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/ggpbmlsgw.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/greybehxe.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/guoylqokk.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/goireomus.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gstuajsik.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/grjfjktqq.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjhowuyxa.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gbkoezajo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gqqwtyfff.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gawwfirbu.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gyfbploez.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gingcjgnr.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gptydsdki.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gstlweghy.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gsehmsmzo.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gvknkrowt.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gvercdzng.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gtawpnpwc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gzzdvigqf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gpsrfyfgh.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gvdevzmev.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gucowpiej.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gvahhiifo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/grmnvbcrr.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.zdbjq.cn/Article/details/gtuxashfh.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gfaukxvem.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gfnyofrfw.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gndxvqfln.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gwvoxlzif.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/glmrlzkqs.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.zdbjq.cn/Article/details/guwwrpxgw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gqpuqbgmb.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/guzhudcof.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gjmgpfkrg.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gymifigrg.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gnhsshvqj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gugxxzekv.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gxlutqebt.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghuhyztqd.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkbiqilmd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glyggqkcv.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/geuvknoni.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gdfzkyhbe.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gfqorqepu.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/grpvwwssp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gbahopqhn.sHtML

JS:   toString() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gctuupocl.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gtmqlgxrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghegphnjz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gvfpdutrw.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/grbppexug.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gjlnbtimk.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gixvipghg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gwplzjogd.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gdfplqwsn.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/geryblkio.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gachgveae.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gbbktrxjq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gxdthbiui.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gzjdnbnup.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gsbalxjzm.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gqygdzdlp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gddxseswz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.hesvh.cn/Article/details/gbjehmpzy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gnqcwuwgs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gflhtngyy.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gmbnhmhxv.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gcvsjscdz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gtvirdkvi.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gqooliqlz.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/grgewpbre.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/grrcbfrzm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gzljezxlo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gzofxajyj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/girhldraw.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/gylbwgnli.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/guqllofhc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gkvwclepo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gxvsuhxlp.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/geyipohgb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gekvdwrbb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gdqdmbypj.sHtML

JS:   Object.entries(obj)
来源：http://m.share.fehbvm.com/Article/details/gzuwmsxnm.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gyfuhpvun.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/ginflgepe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/glnjppfcf.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gfwsegvco.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gaybexqxz.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gmsduvcsk.sHtML


<!-- 参考信息 -->