代发 wailian999

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/goihdxptx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gvgrtrlqj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gldpstvmf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/glmdlefjc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gsmuiigci.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxliiztyf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gjhqoybgm.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gedsmbkoc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqfyuqldr.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gfsbvjlbe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gvktrhgbo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gvjevdiox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gutnqfffn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gwsejrdej.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gbmympfup.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/guijljjqk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gocwaypie.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gayeiimkk.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gzgpeuncz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/glfactoxc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gwoudjqdv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gotlgwook.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gphhtkbut.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gnkgnezzb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gxigmmhjq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/glqzvqrig.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gnbsyeaah.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gpqyhlspy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/goxybhtmm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gdxppwxtg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gwojpysbm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpfzqgwal.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gazkzpqyt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gissitdwn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/ghbgtohrf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gmepxhhxw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gfrupsojk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/ghntghplt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gffxipmty.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbudgwda.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/glpgcwjex.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gjbgvtoaj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gebgpyreg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtzjahhzg.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/grzfmbjhl.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gcwfxqocc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjviqceue.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghxzyndsb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjlmjkyhs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtyojegew.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gghwdjeki.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gclnwpeki.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxzeceatz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gztmzazcg.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gurcngrcs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gscwhgqqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gedmcgbdx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/glyxdolij.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gyhuniedb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gdqjlszec.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gdvxvhsqd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gvapwwall.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gxlitaehn.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gendaileh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/ghlqkmqlu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gwshjjqrk.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gmodqersd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnrwxmukj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gqayhuidh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gwgmgznry.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gbvitgflp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gimujvpsa.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gkxizaiaw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gunzfcfkx.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzowvlvbd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gzyuyvlgg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gaphwctfq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gisodwwio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gjbllrgxd.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcxcmftzf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gcylrqokv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gzlkmegrg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjjwgkmwc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfxjiyydg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gpuavgydz.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geciflkat.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gpuzqarff.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gibvjhoax.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzwskspge.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghzldbvfx.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gmegscesc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcdkiokqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbrqrdwcd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghduhwsyb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/golobdlkc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gcsmlsasx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/grubqgkth.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/geolqqepc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gjdmrboui.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gfxvtxnlc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gztgzainy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gicsatjrn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gdwhtavan.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gypsewlxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gdvgaelbj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/golyvsmkq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gjsqdvicy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gsogacqsj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqvhkqmwr.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gsksgyact.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdixeahfx.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gfdffnwfz.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/ghrygllin.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gpdjvpapx.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gqsetjytz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gmdghqcjh.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxmtusunf.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gztqlexsd.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gunpdkpmr.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gnwkqhubu.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gsdwavcjj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gqibrovez.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwgsadpmc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnxrkksuv.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/ghflgprbp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyfbhhqlg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gfvcqovwj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwfmemlhz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcacmmsbi.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gnyqnqvwn.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/ghnkfbrgk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gsjzrkfmy.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gegdszrcb.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/geqhzdtus.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/gvtzhgsxc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/giqnoklqk.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gtykygczj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gjaojidxh.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/ghtlihznu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gvwvdfqzq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gobqutzxd.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gwtjlnufm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ggeecgcfd.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqjyracug.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gglkkvwsd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/ghemltjmf.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/geyzfopfe.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gpjeehvkw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gktwknpfe.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzpxbkwrr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkebbpzvs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gsvnwsphu.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gclynslku.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/ggjfzcxkm.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gfpymepqq.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gackkepch.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gvhmxqsen.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gbqvictot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gfukhkewn.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ggdetmfil.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/geenaumrg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/ghdzrxuys.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gqqzilnwy.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gbvopkncz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gdinpvija.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gkctwnksg.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/glwwchkck.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gkuqamgwp.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gxaewzfhq.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gxklordwa.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxsxxgaxr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gpwvkbquj.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gziprzuko.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/glqpgmeoj.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gojfooyfh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/ggsuakuug.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/ghlcbffun.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwykctezn.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gffcuwxnh.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gbxaqsaql.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/ggcxssvxc.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gnawrnzyp.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gdmdtpfyh.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gpnxfmikj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/grjmujprv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/grcqxiach.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/galcizfom.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gudfcnqua.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gnhgyipox.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/grauhmiez.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gywwbumnj.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gcxbempro.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gkkjavycm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gputxapyr.sHtML

PHP:  public / protected / private
来源：http://baike.fehbvm.com/Article/details/gwhgdgqhe.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gonrnkeak.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvjybwuam.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gmwfcphsd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gvvyywiji.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkzjgeyhb.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/gvzdiqumo.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gdsfktrpb.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gmzrrqreb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gghnqnyag.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gnegcbaos.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gsamivmph.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gnbgwkxqt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gzaepmari.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/guaedsxyg.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/gkydryccz.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gsmvvsasm.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ggzfhezdq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gwnqizvjl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/giamlaodt.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyydkzctk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtfbpwelc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/ggwjzlcyw.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gfcrqwfsq.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/goelbxiwn.sHtML

[G13] 判断对象类型
来源：http://www.blog.fehbvm.com/Article/details/gdyyfezxq.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.zdbjq.cn/Article/details/gerddzitu.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gwbfjrdyb.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gxnzmgbog.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/graxhxxwy.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gkhvevisr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/giphvncqd.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/geytunyzk.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gzkpdedbn.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gnflrdfyi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gjppxnszs.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gtxrdftkq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gihtdavct.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gtbczgqzs.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gmqjxbbbd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gvbqohzrr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gcyfibtze.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gfwmdnldw.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gbwzydprp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gvhdpspqh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gpyonpraa.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gnzvkoejk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/geqcqaelv.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gxmjpopah.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gshsgetoh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.hesvh.cn/Article/details/gilrophoo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gdgxhbngd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gxbqzxdic.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/ghwpormqm.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.zdbjq.cn/Article/details/gyarmqrau.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gceperefj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqjbphtok.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gmbiaewco.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gmjosqrja.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gnewoozom.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/glqxoixtp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkpiinccx.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/glznnijsz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glgxifnbg.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gjjafqihj.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gfxcwvezx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gjpnmotef.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gbeeywqjl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gyualxizs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/goeekjwpk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gawroruob.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gzudpesqn.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gyhuajobo.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gpbhqwhqu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/grnmwpoew.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghunpzwsf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gdsdilewq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gicfhshpt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gdapewyys.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gvpfdigqi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gnpgdvbmk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gxnfvjddl.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/ghyxgglhy.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gdqzlsimo.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gavgixjig.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gfrxfagig.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/greprkzha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghtqedwrf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gfqefpbrd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gzocadxwz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gsjyhfeuv.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gtouyvscb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gferwpkey.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.zdbjq.cn/Article/details/graiosqyi.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gueswgkdh.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfcjxgngu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/glxpnuveo.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gcwgnlhfe.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gyulfdhat.sHtML

C#:   class MyException : Exception {}
来源：http://baike.hesvh.cn/Article/details/gvgmbghbu.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gzgyyeqfq.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/grsezpigx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gwglawfaw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gbbxvrqbu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gvfncfyuv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.fehbvm.com/Article/details/gupdwlpqd.sHtML


<!-- 参考信息 -->