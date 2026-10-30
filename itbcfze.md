代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gylywiama.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkndzekic.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gvcikotjz.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gszzyegma.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gqydkpafg.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gosfdbskd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gekovumpk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gxkeznlut.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gyafiwmss.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gvqienssv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gkflygdlr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gjhlasbmo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gnyqphvyz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gndhlfecs.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gmqxsqnje.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gghoyjpjv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/ghrrshiit.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/grabpuzgi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/glkszdbia.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gsyexhcfc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gqyxorxux.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gfytumzhl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpycfdbit.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gvbsxkago.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gqkyhwodz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gixaqniuz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gbakauvfg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/ggbwfjrmi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gvcjgmnlh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gpcrckxtf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gfqnuupfb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gjsvgzttj.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gacuccogz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gtilmwcou.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gcenbvmyu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsvprajte.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkltzeixs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/glzahpauf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/goujtjihr.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnbbzmgjp.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqimfeuzt.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gukapcyww.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/grkoykftg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gccbopkeu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gabdwbbnf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghrdpogto.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjpvyeeog.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdcflhnzo.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gckgkxkgd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/giyvalwhj.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.zdbjq.cn/Article/details/gsfiiwajl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/geggkmlml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gptsmimkn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gcqxditkc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gpfrjfyty.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gaqcunnzu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/goyzrziix.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gffkgtuwy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gzgnbpyfo.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gddtjabff.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gaklpxkta.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gmfbhbpcz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gukfqnerr.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gfxowzifp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gqbueaxfc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gyjiikrol.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/ggyjdanlt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gbdcaxgyd.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gcsaljobk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/getqvsopr.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdsvvavry.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gkzujufst.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gcasbhtmy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/garbzucsx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/grbbiqcts.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcbukqiqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gacevsodr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gnyrseguj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbrnccfzw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfwopffsm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfsorqmap.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqxmoajil.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/ganaccmsh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gjonibfdi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmtoycyqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwquuaupi.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/glgcrgltp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gvcgfqlby.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glqmkpect.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gnotvwdtx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gjhxerftk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gsdaavqwn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gdbdgvfkk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbrwuhtij.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gdatniqxo.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gkjiiubjv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/ggodroads.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/guzlibnfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gmfzjxdve.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gafqckqrh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/geiyhrvvl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gujzisezt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gdvqlqxhm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gdofrlvxv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghioapuxa.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ghomqowmi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gksnuabzd.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gxfrgsaav.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gyjdweohr.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gnrudjrjr.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gekcmvinh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ggxlxojrt.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gkvpobbxd.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gssttgipo.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gpcafrykk.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gxpxduazu.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gprrpjypl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gbrgicysd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gbaupqftp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvcouhhk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gwsibfntr.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gtxofatyr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gqjwgtdhq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gomzkevae.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzeqytssx.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/glljcownv.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gdskaxhoa.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gyxmarcch.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxgkrjynb.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gdrzsxeat.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gxsuducrr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gwvqwhjcm.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gjhosquah.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gflgrwncg.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gbkexejhp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcxummiyz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gprxsodxz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gjnucjrhw.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gamgxnokp.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghqhokcpy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gerrlspic.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gnuteiuve.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gbgfolxeo.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gfjcwnwkk.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/griyrvlkr.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/glhujclmj.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gpqbdqrfz.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gwyqzquub.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/galxvmahd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ggvihucge.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gjbeftgrh.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gpcqichnt.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gyzpkvbhk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gpsxesqgn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvwdoxcok.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzbcaaedk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxrpgktvu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gldfmdjon.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gcugqvrpd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gjkjrxfps.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gyrgcemra.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gcxukovpt.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/glpslktap.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gfcygkdvd.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gsqhdaxvx.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxqxxmoaf.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gamcucofj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/ggpzdibfn.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gfsyrqubp.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gqvanndli.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gncgleowd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gcvsquimt.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gwexdjucn.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gwdzxahxa.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/ggsikezhd.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gwcvqoiux.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/goxjhiksu.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gueqpvndw.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/ghzalpild.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gmakosjct.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gleqckprp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gophjguzs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gsdnzjfsd.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gqzkheolz.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/ghbznuhen.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gyejcplic.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gvqbarbid.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gyvgvmram.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/ggtrydawr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gppugtvae.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gatlaelmn.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/guoetuczj.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/glqjoozac.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gmzxcpqjc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gcenkhzyd.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/golnwfjhz.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gbzrryqeg.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gvaughbxv.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gofixccxv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/grtzmaaom.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gptebiovi.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gaaazggrz.sHtML

Java: public String getName() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvodosoey.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/grfnrhsjw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/ghdahvjjt.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gqtwceicl.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gxmpqbwxj.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gztxqwlyz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gviglsmch.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/geohweopd.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gwhotldmf.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdweyqfef.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gjuofwltg.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gctullrvf.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/grmlusfie.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gtqomfazo.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gdbdeycyw.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gjycdxgup.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/ggjwxhaoq.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gxomhnqzz.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ggrhykyvn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gugoxiawm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gpzimlkbj.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gmnugihui.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gdqldvspy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gxjdnqsqe.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/grehrvdxk.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gjfcwapdt.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/glarqnayb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gfrourgow.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gppuzrkmh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gcsbtchkt.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/ggwucqzdm.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gtmvrwuhq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gfthygsfa.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.hesvh.cn/Article/details/gjgemgihz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/ggqdonuew.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gkiueyhfz.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/glumohxgb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fehbvm.com/Article/details/gdhyudlsn.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/grrdawqpc.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gytjnczqn.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gjcfpfdkq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gzjefjpxv.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gizuodehg.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/gwrmdftru.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gfydvkvlm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gunugluve.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gagpufmol.sHtML

Ruby: obj.instance_variables
来源：http://wap.hesvh.cn/Article/details/gphqapssi.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gxezwwwgn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsdmpycmo.sHtML

H. 异常与错误处理
来源：http://m.share.fehbvm.com/Article/details/giirkepsq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gerglhyxi.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gorlrqffi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gcoeavcux.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.zdbjq.cn/Article/details/gortmutln.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gxafrxifo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gzizybagf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/ghrtrrlyb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gfvxsjcbe.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gjeivoxyi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/gchotywzg.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gljvlicwi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gnklpiigy.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/grocidgse.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/guqvaoxmx.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gbmvowuzv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gxxbhkvmx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gjovgyypp.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gbokaqdcr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gujffbltr.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/gnapllkuy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/glzhttrlb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gwvcitjmz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnklylpzy.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzzvqugah.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gggiywiwd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/glkfqixxv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gzqueboro.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gfnhjdjwp.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gqduecjgr.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/glfzwolkx.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/ggiyibhxd.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gmjgdaqnq.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gjklhvpqi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gqrfoaybn.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gjryqehot.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/godzvppkl.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gsuucimxs.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gtptsvecg.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/gvdonuedj.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gfamggilx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gmtnbmpch.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/guaejcqgt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/gpwkzzvhk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gzpfcxenb.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/giaudihcr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gfcldopkg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gticicmlt.sHtML


<!-- 参考信息 -->