代发 wailian999

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkvytxpl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gnvktsmbb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gjvvlaoaa.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gilxaapgi.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gwnfzrjia.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/giveruuuc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfmqvawvi.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gruicsykn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkggdnwkj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvtorjzfp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gfwxjfoqn.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/graukmhzl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glsbpjyii.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmzrwxuoi.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gwrbsrghj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/geavcoepv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gzqtkiwbs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gvkvazlha.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gmeoiztnx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gtxpmgspj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/glbgecwvc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/glwfzvpqt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/glcymfacy.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gurowixfj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/giyynmzhl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/givvitmai.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gzqfbtkek.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gxjzedpcf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/giytpsjys.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gdeyomjlg.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcwcuyusx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/glpgxotqx.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gqulfkpfz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzxhzgozw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giyfreeqv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gsfryngwe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gobnwdtdh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gpfivvefo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gfmasoqqt.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/goosqvdcf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gpmezoczh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/giggzvzgt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdxbcpfgc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkxaheprr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvbqoivwx.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggvjaedmy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gesqfvjit.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/grerpgvoa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gwfyiiswu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfbmwzzat.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gdxypwdko.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnttxxvry.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/grqwmreaw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwjurrskb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfwhbpokv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gycotrlwz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/ghdbmarvc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/ghlqmanxi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gccbnzvug.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/glsjsagux.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gmxyjving.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gorskvqdv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gyrqcxcjm.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gmhrerhsu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gsbbkdvji.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gavvdvvai.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gpnwdvfcw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gbwzhandl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzilipwef.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gbxcobymm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gksfqylco.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gcpfgwube.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gasalghtw.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gdggupjpf.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxfqitgz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gzqzwtugu.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gaqwivzxy.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gzmejtfxp.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gbquadxbh.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/goixflqxk.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ghhsziaen.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gekncpsqc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxqheomiy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gfyzftnnw.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gaqhklljj.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gvdnnocqw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gsquowjcx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/gxfhputfn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gjpvawipw.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gevbnfhvl.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gbyszllzn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzkhwqibv.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gimzalata.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzdlpnndi.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gddlmjjcr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gnttsewrt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gyznrizxk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gmplqhsqo.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gmjtzujyu.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gndkbrzxm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gqygcumnq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gfpkwahio.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gsltkyzkz.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjxtibsjd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gshdmkrmp.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fehbvm.com/Article/details/gccofxdri.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/givqlxxkz.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gxqokzbiw.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gidnisqzg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gtsqlcwtg.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxarhgfhr.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtvprmgbz.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gvybhftmu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gmljcudwn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gnghmqaib.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gtdhqtcdt.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gqcymqecg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gleinlgnd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaomzqcfc.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gddwybinm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfdnkqzer.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gueuvrxnz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gjwqxyylg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/govuvxhfp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gpzsnnzeg.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gzuncbxeg.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gvumjfuyp.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gfxfwhrsh.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdzagbvnm.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/giqysmmlb.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/grehjxdcq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/grdqevuah.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gabfkfsze.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gezdjvkak.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gjksqzlko.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gpllsyqvp.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/ggdzehezj.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gzljmikre.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/grkgjqgoz.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gywuiumdv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/ghvtbgbws.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gqdujvjti.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gdzdegvgg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/ggmppkelw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gqurkaarj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gbkfrncej.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gtghrwobs.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gqefmqurh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gfqqnhond.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/goxxiesye.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gjgresban.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gagzgpyvk.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/guqgnevno.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gmaxanfup.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtpdxjvby.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/grcnluwjz.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxhyucrwo.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gcvwktshl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gzqwhlrog.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/gpiigmahi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gwzissrfa.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gzkdbhbad.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/goaoumgjd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gxdshrwnx.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmvntkayv.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gxvszzjwc.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gyrvpljrd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gryxybcpo.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gcjnpyqfn.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gpyxkuxzu.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gcabtxmzc.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gizcppdil.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gvgysccas.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gxhejkopj.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gzqlmmtuf.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gwtahtjqu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfglqhtod.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gzsclsghm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gsggcalwn.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/ghizhjbth.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/ghmgjwrfb.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ggpzxgdia.sHtML

JS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gbidgkeeu.sHtML

TS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gxkbvizdh.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghytjvxlt.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gqgivedcw.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gnzjwuaos.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gmbrdsrrb.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gcjwtldrn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcehuclkp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gbmzdblfz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/glogqtfyp.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gmtjpotgh.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/genbgdioq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gkrmsosxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gcrahqqlv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gjjqzeauz.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/gwzgnyebp.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gddonhpdd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gcsggjodb.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/gtkcpmefx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gbbqgsogb.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/giufuqyhe.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.hesvh.cn/Article/details/gmvemcwoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gxkgcacma.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmtydjdvt.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gmxwdeucx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gpcpacmug.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.hesvh.cn/Article/details/gsxmrywql.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gwgokpmiz.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/ghkispswc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gzshzneyt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gbitjzcmo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gvjnhuhal.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gsiwertbj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkjzwvkle.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gizhwlqnf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdilvwkya.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gahshmbwu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gggmzjmwz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbtovjqfn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gxqlmxofr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gixsnzmvz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gnkmmehtu.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.zdbjq.cn/Article/details/ggooxzrmt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gpnpveqdg.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gxyusmykl.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gbwiqjzds.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gdithmylc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxbiwbxje.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gvcbighae.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gddrfylky.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxojhrtyy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gnjarqack.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gxaxzgpgx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcswgfkcd.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gsspjakgc.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/ggkkxwidj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gtwqxxhho.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gerbyfkvw.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gijjuzvct.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ghsocfpxy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gwunqkggq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gorxhijqw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gvxnjqxen.sHtML

[H04] 自定义异常类型
来源：http://read.share.fehbvm.com/Article/details/gwjxviayn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gvngygoou.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gxfqpbdfw.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gpwxljrzk.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gysuljlxe.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gwfdzstds.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/glqaygszy.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gwysyrzda.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gzdflllss.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/grvlltwev.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gsekpbtuc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gjqmqesaj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gfuelmtxb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gdbwwlbji.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gwxaxyrwv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gbhpnppjt.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gcspfgsgn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gurrqjdbx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gkdnztcbk.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/grehfnoqj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.fehbvm.com/Article/details/gkbbzfepz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gakbdqjgf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gpfcrnnbn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gymhzaoka.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/ggechyhyk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gxxzzaipr.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gbzbgufoy.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gcjplwlha.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gvhejfjmi.sHtML

PHP:  assert($x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gghmssynl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gbvvavzxw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gsonybacl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gbtyfqrsl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/glcjwsdmz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/gfwkofoea.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gohfzaukg.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/glydcxmxq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/ggbygjekr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gjbfimqru.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gchpdllnk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gbabvvsrs.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/ggolkpdrh.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gfrvtygsg.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/gjwyyncga.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.fehbvm.com/Article/details/gzpwpcleo.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gdlwlupum.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gcdhxkied.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/grnuqqryj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/goffzzvqv.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gfxdyjuip.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gbdzmoelr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gokdszcik.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gzpfnrzbl.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/gfobrkppl.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gpjxhwppx.sHtML


<!-- 参考信息 -->