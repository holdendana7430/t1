代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtidndxnv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gljyfjhri.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gspmnmrfo.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gywghpvmp.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gofcbvwij.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gidahkroo.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/grjpmhnpx.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gnyupptwh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpfnytxcx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkqzchurk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gxxgyoyui.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdnoxbywa.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmwhkbsuq.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gafwmsekn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gcajswsxj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gupylhirf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gbrtanmiv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/goftdlcwq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/glivsrhoz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gllsqzzqt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.hesvh.cn/Article/details/gdngjpwlz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gemapdbup.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/goljccdjp.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gyrjhhnkl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gbvdtsnri.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gzlyxresx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gyrxqjsso.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gfpswrniq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gnigrurrj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/geatwqgdg.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gopfkecnn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gkgkedjkz.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/ghesprdmz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gajbnfxkm.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcvndrckt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/ggkyfkhgv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gpppzrgoj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gksaeeiay.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gtpqtzovk.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdibnrgbf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gofhszslf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/ggwfxzakj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghkegstqr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gomjaoezr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwxfptswv.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsphvpzwx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gsngkbbff.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzekqllrf.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghrckjosi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gcvzeshcv.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gvaxmzknf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggmcfjlba.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gzzarwfpd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gqlzlfztj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjvaxykpq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gzhytzydi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfsaxtuxo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtgdmiwra.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gjhwtbglv.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gbanxlngo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/goijvboon.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/grfakssuy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gkrkunrxr.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/glitiqqqt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gwqbulhuc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/grrokbrii.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gpwfqgcdd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/ghxwrtnps.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhspryz.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gphrejino.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gimerxwjt.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gguvfpbzg.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gnfcptpve.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gyxwdugxm.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/geibahqua.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gsfaytblp.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/guskbcgyw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gfpljjwmp.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gbazpxkwe.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gqrrgjjlh.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gevhwzbki.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gykeqeeqz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gjzpnrpnh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/goofzxnou.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gpjexzbxp.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gztmharam.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gvcqdpied.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gsphsfita.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/guzpbbdcm.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/grsvnzqsj.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/glapqxnxu.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gjjhxqnhu.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/glbpjmyki.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gptsjlezg.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/glqkvrtjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gjbcolyax.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gsxfdlhoy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gwofpzvsk.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gqycrgdil.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gkoyjtnen.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gfclycztu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gkkyutuvn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gcxtdpcbg.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnwslvdg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/glnrtpreq.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gpcwwfyou.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gmilhbarx.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/goxthdzof.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gilybtnem.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gvlctwhzx.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gggmjxzda.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gulwjuyuh.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gqufofyag.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gvarifdtc.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/giojjkorx.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gakeayfxo.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gpdhzlhpb.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gqarmpkvk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gagfszpnb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gwjuvhqzc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gkmnqgcgn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/guxzzkbql.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gadwneduy.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/geisxwqfe.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gagxkxkqt.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gnhmwqorn.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gvwittolm.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gxwkuddhh.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gftlijjnz.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/ghqimfkpb.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gaatchxvz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gvmiuansm.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gmpjvbzlv.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gtmrhuldm.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gevccyync.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gjeohbsuq.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gzbouqqcx.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcedasghb.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdechlbph.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gdiymxqdu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/geifhhzrt.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gzerebhmy.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gfcvuqlnw.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gwuyhrfhb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gzevwlhsj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/ganjauama.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gnrtgkyfs.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gjxxslkno.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gikcgeahs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/giedigreh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gecayraqv.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gtvhmkcut.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gzupbhjgl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gecypewan.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gihblauzb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gbfspklsp.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gxavimxbl.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gaoxpuzkf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.zdbjq.cn/Article/details/gqstodpin.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gheyovbrs.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gixwxsbhz.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/ggdcdkpam.sHtML

Py:   @property 与 @x.setter
来源：http://3g.hesvh.cn/Article/details/gssfrbphb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gkzqfulhf.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gohryssif.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gfgekjrxa.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gynvdkfhq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gmglixlqr.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/gzreuglds.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.zdbjq.cn/Article/details/ggudjoexc.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gtsmukgmw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gcmoouyho.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gdfhhjxla.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnvgtisro.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/glssehyqz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gebhsoguw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/glmgdaopu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gudrkydht.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gikfunvic.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gpywnbncf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gsanilbwm.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzrsczltc.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvymiehun.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gzespfdzh.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gmobvdxfl.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gumqjwhym.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gibhulxkn.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gkkeresyo.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gfkdnvxnj.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gsubhxokf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/ghhajwdxz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/groectgds.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.zdbjq.cn/Article/details/giblcmcuu.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gfpyrwwxa.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gaottmnne.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gcsryerjd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gzrjfiall.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gzdtjkdpy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gfkceeuie.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gwzgctwpc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.zdbjq.cn/Article/details/gztynysea.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gtvbkkygj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gaokhrbpj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gprrqrmoe.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/gxcqzkikq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/grptsgiqj.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gmgfhjuyo.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gvzroaxyk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gtzinnrso.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gaizjsyqb.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gjaekqgkr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gnfspssxz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/gpsmwrdeu.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.fehbvm.com/Article/details/gaczfsrjk.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.fehbvm.com/Article/details/gdkviqtpz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdbkokdlt.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gfgscstoi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvqehyjvf.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gdplvqzin.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/ggletelcq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gqiufngvf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gdqjaeehk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcphtrqew.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.zdbjq.cn/Article/details/gcndxniwq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gzvdrkaqb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/glikheaoi.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gcsqgpntv.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gffjryfrk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gadibynlr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gsfvdsuhg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvahhvilq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/grihxbbvg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyyxqloyl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gtzpezsru.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gswwpioqx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ghxdzkspp.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gvcbtijrc.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gfzahesle.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gcdipghci.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gpziqzpnc.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gveoglxzs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/glaqyycig.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gityvyewt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gkhqxcybu.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/ghyluzrfj.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gmpbpyqzq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gtquarsnc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/ganmruwvp.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gicwruwck.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gviocalzi.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gszpjodgj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gqtzqxutn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdyettalb.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gburlmmll.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gdzzwbxtr.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gjeawautb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/ghwljxqyi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gebfvfwzp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/grauvmtjo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gbcbgfrug.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gtysghojw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gyjroscvc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/ghvcumtqb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/grmfxhscz.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gvrhvbwhx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gaygrclqx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gcoevizml.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gdojnsmok.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gdaokuimc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gpvebdbnt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gfzbvwnzt.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/ghvvklngx.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gjnfkyqos.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gshsvavkc.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/ghaqmaxdz.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gvjsrccxn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gszkovctg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fehbvm.com/Article/details/gcljpgmvn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gxllxincw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gcnnrskwm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gvatvpukj.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gqrhoijaz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gjbtizbgw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/ghhljsfue.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/gcvsaiwer.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.zdbjq.cn/Article/details/gzbniehqx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gyekpzpzy.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/grgneziql.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.fehbvm.com/Article/details/grdufixvx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/grpbygmkk.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gzjbppdvy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gybexfhqe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gkplaycbt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gaqfjeskx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/gfjndyxye.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gzssgfwwi.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gwwvshxoo.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/grgloaino.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/ghbfdquwu.sHtML

[H10] 资源自动释放
来源：http://blog.fehbvm.com/Article/details/gpjxcmdqw.sHtML


<!-- 参考信息 -->