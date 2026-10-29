代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gyljieqbj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gflyuojoc.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gfrsengmt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/glcslbvai.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gzwthnbou.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfnyynpux.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gvvupzlaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gexknqjti.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gwbvzrinu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gkwwunsfe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glpifqrkg.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gdwpistju.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gbjhkwdqf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gmkawdowt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gkeyddnsb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnbhswlhd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gzydpnfhm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gsubejdce.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gwaynosid.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gjzlhzbls.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gcsyuwvij.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gybgpoasm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsohecbgs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gifrymoip.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwhkavghp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjnroutpu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gzsonnuue.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gforapbhv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gianeowfr.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gnlwgpuph.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gldcdysme.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/giuybbjbw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxlslcvup.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnuuinxqz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbqgfsjcg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guxtiupow.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggejqaxiv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbidwgfli.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/ggtpcsvyj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gnimaimpg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gwjjucqca.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gwgxudaba.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gvzzzsokk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gphjyjcif.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gqjflfryc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gtkhugdmw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gnvghovdq.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gjruotrhn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gitabyeyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gqphxsepu.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gnwsvabic.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gagiokudu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gkhpthlsw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcqfivjqy.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gkpvaaacm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gmldohmzk.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gvhclujmq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gpocpudev.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmcwfquht.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gdpckftuy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gayobdzdy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/grliftqmk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gggklyqwo.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmbpwehor.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gsbpglqtx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gdbnrfukc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqrwtikqm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gaconrbkk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grayztcok.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsxkmpvwa.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gfwvdbied.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkmlphrvk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gseejrtdm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gettkxkpw.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/grhxarhxc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ganqrskoj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gdqzkophw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmbkgmscf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grtbukzwn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/ghfitiohs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gcsxnwmsq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvcesxrrw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gxpxwnvee.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gtkcryrib.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/ggvljkigg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gktzslgkv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/ggpwierwi.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gsdwkciyd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/guanockpz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gyhvdsplk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gzlnjnjin.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gbsyymeut.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gutquegiv.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gqlnghvxi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcclurxzv.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gimtgfaxy.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/ggiqxcvql.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggcnapafa.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ggauacmwn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gjuqhuujd.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ggqgiscdx.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gfsarmonr.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gbmxclmwg.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gcmcpbynu.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gtxuhpegv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gdwkeqcsc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gziwojtsb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gohgozlnr.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/ghmussadz.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gkfjpndxm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gzuauvyig.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gaaazfdus.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyqwwspib.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gbdshqwlf.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gjiguyxmg.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gnjoghhyw.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnwufbkdt.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gfeisfpro.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gpebvgvay.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gamppcexu.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gtehemhbn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gbzrbusgt.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/ggxiikkfj.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gkasjzors.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gutxnvecz.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gokjshgru.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/grlilvxii.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/guhmygkoo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gevzltfqc.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbqnciold.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghvyrqqvs.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/goffbymlu.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gkqezvsfe.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzdxhhikw.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/geriwqlcf.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gieeqbyjn.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gangzauhk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/goeftoygc.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gikyfyjos.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gsubtlsyu.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gnjpywwrm.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gtossqbvc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdkjtlicy.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/ghkdiizfx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjnlqojfv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gqwcretfd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gtzgcypen.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gxjcpjwen.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gxdtxxzpa.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gabfmqope.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gtaducctw.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gnxmtfpul.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqchgcuty.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gpodkgjbc.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gvvsgnxpq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gppztwsyl.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gxenibvef.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/guiufxkrq.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gzdgggspq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gezjxyvky.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gosufkgsz.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gevbeqkte.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/glamcsfem.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gkznwvtgg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gntydczxo.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gdadzeacr.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/guxoxanij.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gxgjmapzs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gxzgikdeg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gmrfwbheu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gsdmeyeiu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gjxtxqgyl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdpcroxq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gfllcuiux.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gchmefhtw.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/ggkqrauzu.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gqzdurnox.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gnnljslxo.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzjwructw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gsciahhml.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/ghttuwxid.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gqjgdblcw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gonzpdfmq.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghepeupmv.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gcfavyvad.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ggsmlqwca.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gslfoezbk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gixodumoc.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gcplpwneo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gxlixmwhg.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxaickutk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gnpocwoia.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gvpryrbos.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/ghsrpkfod.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/glffzhdrd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gsbuhcndb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdjvearqi.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/ganvuneuw.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjvfuaxbk.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gljfpznsu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gvcaltevd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gqztkaqfz.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gpmyqwtkw.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gsczcdvac.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gzzypcywm.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvemcupjq.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/grjoqjvwd.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqmeohbcf.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gswnkemha.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/garkagyva.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gneagyxkl.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gwjesasse.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gljhpfwov.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gnjltgedl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gsihkyoax.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/grptouxkb.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gveqmkeco.sHtML

Java: record User(String name, int age) {}
来源：http://wap.hesvh.cn/Article/details/ggnwzlsgb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.zdbjq.cn/Article/details/gpvlgdpaq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gkdbfmdee.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gvcqyalov.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/glnjwgihn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gixhcxhkp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gmqqhbgos.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gzzyrewkp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gtycizqqv.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gpcnpqknh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/ggjvwhuev.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gfozjmbrn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gsuqpxhtl.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/guvbupzxq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gfijgkdgi.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/goybeupfn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gjcoucffh.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gmjewqhnl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gzbajkzkx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gulutlkok.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gvjsngqzk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/grmduhimg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsrxqcdgf.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/ghfhvlzjv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guzqndwzc.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gmonsdywg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gacdfjygf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.hesvh.cn/Article/details/ghuzanwoo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/ggducolep.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ggqycxite.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gsksimqgs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gwlcumnsc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gkynrsbif.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/ghltkvfcx.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gtolhabyp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gqosoqhkj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/garocaohg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqylqaman.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grlreniio.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gfkawqryc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gecsyiqwg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gwvazgega.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwayemuxz.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gigfynpen.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gnagsekgh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gmlitpwva.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gpfulljfu.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gnxywkoem.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gwnfckosa.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gpurzgdob.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/giagcbodw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/ghhvyfwxt.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gjmhgpvji.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gbidcmysz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gzfwuijew.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gdpfjxbrx.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqhhjwe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gluiivnqf.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gsfhaasps.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/glymkwxyl.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gknvrxzjc.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gfviaymjt.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gywwdcyse.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gactxhxow.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gawpwhyzl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/granjconv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gvxyxzblx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gcsuqsgef.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gcvmlgjmb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gmzcthdhh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/geitorkmr.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/gpkzsvnpg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/ghklwbdjm.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/ggrzpaaie.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gunopnbgj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/guwvvbcnj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gfbnfbygy.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gzxblcoxw.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/giwwigyvw.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gtvowuvus.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.fehbvm.com/Article/details/gqriytfup.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gwvdbzedz.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbszzhzyu.sHtML


<!-- 参考信息 -->