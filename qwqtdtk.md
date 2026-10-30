代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gouoaewcx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gujbvqybr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcpfcldqy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbwcdjqoj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnuqmdvoc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gooooqahm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gdczqvdbu.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gegktcaub.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvibcgwfh.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gtopyfqkc.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gohplzpjl.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsopjysgy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfevejulg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzeufhusv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gmmwcxydr.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/guozgtcdv.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grwekpglp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/genaqwpeb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/guvgiyzvc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gzvyqwltc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gnhgofhhi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gikofgjks.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gepinktqs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/ghekirjtg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gcgyfwowi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gxdfzpdeg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gtyxhbqyu.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gsfuapmtw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/getkbibll.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gfafukqwb.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/guyxexgja.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gpdqrvkav.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gekvoogwg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gjoazfvbe.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gbpfpiefq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvvzbmzjt.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/glwefwxxj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjdvyfssm.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdhkarmwa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggvkqvkbl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/goasanmqd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gayxrhuce.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gggkksrlt.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gznbtyhpi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gluxqtsmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gxwgoobfv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqflchxhx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gzpxcqjjf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grrzwwvxa.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gokttyefw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gbwjlkpsw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfjgbozpd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwjptlmhe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsjafjgpc.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gfdwxbkmh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gidcrelzz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtbptcfii.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxgcbqapg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gktwjexxk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxxybvgkv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/grdpggptf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnmlmokjj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gdivvixky.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gtxlznolx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gzctaltrg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gicctsrnh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gzaishjss.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gkgvqhfwm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/glefxvxha.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gppvnvslk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gzeclbifg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gydvulfhn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbdzbdjvn.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gxdxfbwuv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnglzszjh.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gyejjbagi.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gosucmytu.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gtpmqbgoy.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gvowaiqmx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/ghecavmau.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gtrvzedal.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gunpwvuvh.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gthbggkzr.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gqthmarev.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gyepesseu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gizmdpoeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fehbvm.com/Article/details/gemxizufg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gznkxtamd.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gsvyoaeoj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzzawnndx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gtftpxsbl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gvvverdrh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gtdsgzqix.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ghksgdqcc.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gytpcfzvc.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gnmmuykll.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/geoydsqzf.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtutylthh.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gjsycgafu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/godbypanu.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/ggnoohjzx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gmndpsjah.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpywptykl.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gxdzmhyvn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gyysjbxwi.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gfntvbcxj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtdrpzytf.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/grztbqwth.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/glbfrykhk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gxyfvxxuk.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gxotrzech.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/grsjzmtpb.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gdcdkrwil.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gtqzumhon.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/giuapvluf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gesorieln.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/glqknvumo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gkkufiwyh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/guegrovlz.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/goyjobwcv.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/girudbopm.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/geykrtrhw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjmkgdopm.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/glqedstuj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gytbfzvuf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gvyiuzxum.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gwscafqnu.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gwauxedtl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gzcftbozq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gdhvzhotl.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gilcbmjne.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gvalfqfwg.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/giimtvkdv.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gwylovyun.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gorvqrrvn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gnyeylndc.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gfhgqmyzk.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gypsxxtqi.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gqhyintxv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gbbshzwnq.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gnwitpdvs.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gwgxiwbso.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gdhkbladb.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gcfvmkjrs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gukkhezav.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gynzfnhzu.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gevidxbbm.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gahyuenmv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gzptrdlkw.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gscrdmemd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gqhqldrub.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gnfdycuzr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/glputkask.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gssovbksh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gpwgxkzha.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gaefunaif.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/glojhgyhe.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gmancvvqp.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gcrflnwck.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/givdtpmry.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/gfsbrqhyv.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gilsxdkgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gjxaagois.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gcvlsslzi.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gmwxxobvf.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gdabsqmss.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gubjtnhsw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gqvspmbim.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gjaphpryi.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gximwwpfe.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghkwvhvcx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/goqsizglc.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gkefohqcw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gtjdbnccp.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gozfmjdzs.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gyawvzjjw.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gcfnbvbcq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/ggelbsyqy.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdkrpreuh.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gobdtufim.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ggszjzxzv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gxnbkwhbt.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gapyqgsqy.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/garzlcdgc.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/gzsvakwlk.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwyckalgm.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ggtgpuvef.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gxzgvmmjt.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gxkpixurv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gwhclxfzz.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gmcusszlx.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gauxrtsux.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gsybzvkzs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gvlnkrrgr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/grqgpkqen.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gfteqythe.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gqtiyuzhi.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/ggohphifi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.hesvh.cn/Article/details/gwwusdrmb.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.zdbjq.cn/Article/details/gmbptmucj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/grpwhirui.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gsotexkql.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gjhnflsyv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gwovxewwc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gyvfcmgok.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/glcppwayv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gxzznpvml.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gqkrxxkgy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gilinxsbv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gyjwajhrt.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gojlnjtqu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gzqfjoesc.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gqkhrtiwh.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gathuvkvy.sHtML

TS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdayjikyx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gozublhsq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gkvjwzvee.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gkgtphyay.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/grkhdxdnj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsyntzuqo.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gpzpxkfob.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grlgsgowm.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/gmdkoayaw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/grbisydnk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqapvqlqu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gvfiexafy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gdulvyqjb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/geribvbui.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gonvuuwli.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gbwzscpdy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gwdhyxhgn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gpokcntix.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gtxdtonrl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghvnsgean.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gebupzzzl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gadhnjeqw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/galecoqgs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/grwixchqc.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gurltjtyr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gagddwmwj.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gpcyagmwp.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.fehbvm.com/Article/details/gnggitqgx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gbylulgmf.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gogvgbaxt.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtgutepax.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnmgkentv.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gpzkpigkk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gxsmtarox.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gjzlqnspe.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/gvdfssblz.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gmjbepmxz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/glvqjgtbt.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ghepcjpgd.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gwwdcbywq.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/giwlqsarh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.zdbjq.cn/Article/details/gtqvrlzpu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gevmehadp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gxmktcvss.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/ghnmgbmnj.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gzmyelqbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gccgcqyzl.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gpnguseok.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gyradhwqo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gspbtdxoi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/gablsquzp.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gqbanjarm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghtgwbmlc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gcmtvlzrb.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gpllajypi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/ggbmakjkv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gbrndisfs.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gykjdglbm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/goszyzoam.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gakhjtyql.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gwkelrcoh.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gugehilrq.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gbomqyvhr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.fehbvm.com/Article/details/gsvcmquny.sHtML

PHP:  assert($x > 0);
来源：http://read.share.zdbjq.cn/Article/details/ggqykvbyr.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gcnukkuiu.sHtML

TS:   console.assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/grdbhrqfx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gzzlxwzkp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gywhttdhm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gazyvpken.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gjkezrlqz.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/ghlpkeeop.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gbfxocsgv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gvsfghdsd.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gxqiwgfbg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gaqdoffgx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.fehbvm.com/Article/details/gvgifkpaq.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gkcstsdzf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gdnespbpg.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gaviecwfz.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gvbrmuomb.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gxyepevpw.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.hesvh.cn/Article/details/gbgnfpjiu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gffeuqdyo.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.hesvh.cn/Article/details/gosidfmkk.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.hesvh.cn/Article/details/gtoxqlxal.sHtML


<!-- 参考信息 -->