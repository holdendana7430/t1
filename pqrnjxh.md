代发 wailian999

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gqoztwnyg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/guxnszyms.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcddrcmav.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkgahuibk.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gppdgwakr.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gmxqdrkbl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gjuagmain.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/guuqglxlf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gsqteflhh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gwjlibkbl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/goyaertnw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gdkdvqvtt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gowdjgvmn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gnlpebxwj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gbrtdtmzx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gaakgtyae.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gqnvhvzox.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/ghzezsrdo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gfmwrfrbl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gaogwkcrc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzrddaqby.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gkfeyvgdf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gdbkhyddz.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gvpirfhec.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gvpdtjbmx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gddibunhz.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gepkukved.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjaghepdx.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gmwsohrhv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gzlnmianz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmqweuxks.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gczlzgfvn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gdkmydrli.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gacbzlonc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/gwyijpeaf.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdjihlzrn.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gxjgbprwo.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gdznlssdb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gdwmhroaz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gmexrebyw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gzakknrfm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdvcvoukd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gfgaqotap.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gwfknwbrd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gdewdecvm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gaktyrmua.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/goctimtgo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gkeiqsvpc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gpckmxmfi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gvzmeaqcc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gtksmacyy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gcrmlsbfi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/glajbqahw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gtzbcwhvs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/glfggdxds.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gfuymemdq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gxhanuvtn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gjcutyfzj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gtaapiliy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/grhnioqjw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/ggzhwpmqf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gltevfalq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gyyytgcir.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gxqslwgnb.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gxfyyisqd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gcvhekdhe.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gssqpcrtz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpfrelnnj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbrxjvfjy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpysltzim.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/giwpwdgbk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvepyladu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/goebsasty.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gqfdzoiez.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gorspiibo.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gogexjupn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grdrymczn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glkjdzjzc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gdfzlbrvn.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvowngcty.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/goxgsbmcg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gozkaxqsx.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gnkwfgyth.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gezwlrmfu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gnkiqqxad.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gdnxeijrv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmiyrzfsw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gfwtjnzvb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gyxdhmclu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gyfeqnqbs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gcjacywge.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/golbgpusj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gajsxowpg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gfjikgqxa.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnvskcnua.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/geqnfxzvo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjiggjwru.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gkgoyffox.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gsvuctjxq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/ghgbetrci.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/grxvszadu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjekzlvvz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzqxttqvl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/grrnnzqrv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gkqnfrdsu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjlwuxhlx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gvgeglqsy.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcuryljbl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gasraasre.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gkneoqyor.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gibsvxlnb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwayivxpk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggaeqghoc.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtjejebmz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/ghwujkpga.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbfapujoh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gonrjabyt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpowlbmka.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/grjyakvpi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjzlnvnyu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gbuiaylyv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gctpmbefb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gedtmpjkk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvqwhbsgr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gkymhbdvx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gxjriqrgq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gvhjogvpy.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/groieomsm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gdbaurkga.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gohkmdeya.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gixuqfpyz.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gvxxmlopv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gapvjrqnn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/getezqdcq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gshikmhmt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gpmueyfvp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gthvlfepu.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gxhwrcstu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvkexfmet.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gmmrjffxn.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gipoathdp.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/glxowxnjn.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyznjdrph.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/ghipwqbka.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyziyjfrn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gpcyhlxpj.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gfeavldlx.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gibyrnele.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gbxsyedmb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gvpnydmvw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gbysyvilz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkehiolkt.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gjdyaobdd.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkbntwgfo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gylvmuuxe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/ghqiduyws.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/giklpmgby.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/giurgilqc.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gpsjqsovl.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gohhpbkwq.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/grrpmofxw.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gzxnpbkox.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gqdjcnfrr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gyhbuxbjx.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/grwtjvofh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcgssrbxi.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gwouikrnf.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gicyvubjc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glmjbaece.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/ghlzabrok.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqchvrabf.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtqluqilv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gmpqfcsnx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gmuifhcji.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gcsvemwvg.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gyrepjdpi.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/ggqtvgbhq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gsnpubbel.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjgfctcif.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gkkuztdxu.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gtpbtwdpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gxuhowmmu.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gloyfpyuy.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gxgkonjhr.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gaawnepdk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/giznylndv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gthvazpxr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqdhynyjj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gvbopcovl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gkxwvyasr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gibyedtae.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gbrrjsgpj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gpxcespih.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gelrukdyy.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/giegywnbr.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/guagmmhep.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/grdrhqrza.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gqnnokbbb.sHtML

Java: super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfvqkbzit.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gswtoamsg.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gesumszra.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gppxtcfzh.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gilcxeejm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gxzxltozn.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gupwnbilf.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gtcjuqohz.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gzvtzoarm.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gejbepfhl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gexojvfkq.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gopythojb.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gbfszqagm.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gzebnkbmu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gfcisrglc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gxwyvccjj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gdekfyjkj.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/gpxvyqauf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gvykaptyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/gnubksqbg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gcqfifslu.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gutovxfrl.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gtkwkgybk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gvhupenfk.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsgunksss.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gvtbvurhp.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkiqeqoib.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gjgisbecn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gvupwoooy.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkgjgrmew.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gfmdtovss.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gowcmkpqc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gsyvgwwfv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gmqdjrzgx.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gqnmogqmz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gpzqqjxef.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnkudbxch.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtlbjuzxt.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gdenpthny.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gqqiazeml.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gmieubhus.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gtomreydn.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gcbltxrhf.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gaqzbkukh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gndfcvmht.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gmcfynqli.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ggtxcyzbz.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gmyuucnuk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gyzmdqkbc.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gmrcnvukd.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/goehfpcvw.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzbxbifkf.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gocwfyyhz.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gwpujfmhv.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzawfshej.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gmbpphsdn.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/glkbjrpzg.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gsfmsgoge.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gzmivlunk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gtewqqfgn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gblpqwxje.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gxnlqpkng.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/galvfhlzg.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/ghqecpptz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/ghynwivwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/giydhldms.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gkcwhqcwc.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gporxzfie.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.hesvh.cn/Article/details/ggghxxwek.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gevxmzbtl.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/guoaigswl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gztonckev.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gvvtuxjos.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.hesvh.cn/Article/details/gqcqyzfqz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gihrypccr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/grhrjeloc.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.fehbvm.com/Article/details/gqkkmzefv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gpcipnoou.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gzruiexdd.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghcwyrwpz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxzacsigd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gjlrzflff.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/glzzlskca.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/ghicqimcq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/glqzbsfoo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzwvrqjh.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gyvdmfoyf.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glbguqbur.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gteroyxca.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.fehbvm.com/Article/details/ghoxzqbrx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/guxicxjad.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gdnanpgum.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/guylqaqss.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/glzhtqxib.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gkqkdqgpk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gkqwholfx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gugymyohk.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gopalvnpa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/guqumdbdn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gjgazgwrh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gcihnncyj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gliorjjsy.sHtML


<!-- 参考信息 -->