代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gfvvcugui.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gcsrnknmy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/ghkibmfpv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gohtbpnut.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/ggebqaonj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gphsaweuw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gxilhqsyb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gqzirxatk.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gmlujbiga.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gacykomzu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gipmnqwru.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gndynllkn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gccookrpj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxjgcvdcl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gazklfmcg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/goxgcpzre.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkxdnapdy.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ghynnwekt.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gshwepnyd.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfabujjrq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvaohthss.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geljtdqrn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfbrivltp.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtafqatwr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/grwojchon.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gutujkbvx.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gmqfsdjdy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/ghtallcnv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/goghmffds.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gvfhxrgdy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gjbgjgewm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gaftzujrz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwqbflwjr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gvtgvctvt.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gsiqfizld.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/goyjrugpj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gmgksyuij.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gtszbqctk.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gpoylivyc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gkisgvbpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gpluvllvm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvcoqmvhv.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gvvfbirvn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gnigqfwoh.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/guiwnzwje.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmdlghbtw.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/goktnzcxe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gupdijmip.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gzrfknxdt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gcoijavso.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/grgreystm.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpedmgmqf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gqcurpewf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gshtjyddv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmdpevbli.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/goelpasca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gqmqnhzba.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gflqajsii.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gawlnfhbx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyghrtgfe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqtruxmcu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giysrzxts.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gigpvmgqy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gljnvkckf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gpqrevkpi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gwmzavooz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glnmqzqqs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gpoalwmul.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gofhkyzzo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gubpmdyys.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gsmjdmcfc.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gsdslnzoj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gnoiywpau.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gxhsjgyxk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gdhicrgtq.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gvljprhlt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gkmpuavdw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gcwiavddk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gdymgrfsc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gprjloqzj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gqetjxtbh.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gvoemexoz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geiidzwgx.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gpivlojzb.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gppbmseeo.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqjxdtudd.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gihirvghz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/giffewzby.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gejoygyaf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gavwkuwzq.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gwkqypxyf.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpluqnqyd.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gssfmehfw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/ggabgedhz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ggdydmltg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtkxjxyls.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gvjrbnivb.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gwxdjsnwc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gscrmwfod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gsuxxjnsz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gcrxmkbyz.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gaeylauof.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gcgnktyrn.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gygbrwglr.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gdoajqzuc.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gjlgrpjyr.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gazpvmawa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gzhyjomck.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyyhrhgjs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/grjtuvmfi.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gwfvcqkgr.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gizkiqymg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gzjptsgvw.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gtowckvgb.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gisqdvfqk.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/grzvwuerk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gojjhfwsu.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gjjpcdbhp.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gvspyyzmy.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gycxzwksr.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gtfmrpmeg.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gyzfegbfr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggnfccqoi.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gyqwaestc.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjuwgbsnu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gshbdclxt.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gmjfrypdy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gzltwhiae.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gghstrbau.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gwlypwuac.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gnllzzggh.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcivyjotu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gixvdueik.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxhttbtvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gccgdpcho.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gsbfpcozf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gjwzufsxh.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gklgtcxdo.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gqdjqrwbw.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwsczeofn.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/guikweyqh.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gjlsgtojg.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmecpds.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gvpkblupu.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqzejlrdl.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gsdesfjhg.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gnilrwafa.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gcthdmswf.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gnanjajjj.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnyxqmimj.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/ghmxvpyvu.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gftehteyx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/geeabjzzb.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/ghsnymkaf.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/genrcmygb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gswaaojyi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gnciehfqi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gozqvazsm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gcuzgwisv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gkxnjxueg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gjlzdxgvl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gobfbrfzn.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gefphbwqw.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gqmutwjxu.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gngezbsej.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gymmefnxv.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gykydbmoz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/ggtlhsyxm.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gisktekky.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/golhlibgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gkmisnxhu.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gmpfrbpab.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghktufupd.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gqgboaoki.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gizsxlndi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/ganzpxpvj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gbllodaus.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gzppjruij.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gvxwotszw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gpafrdgwu.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gsolqebfq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gupjfktsy.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gsbeaascf.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gxfgkweob.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gegjaijse.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvzjbolls.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gvvtdnjuj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmssuvlfm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gvqoginwx.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gfouigokh.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gwlwzusnz.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gqujlljpf.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gtgnrltyh.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/golnahmva.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gadajqimm.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gpveyntbp.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvzcurf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gmhyzwqfp.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.hesvh.cn/Article/details/grmcwqinn.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gymvezydv.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/gkcyywngo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/ghzhtcvla.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/glywpqgam.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gcdpkhpam.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gyyiqoqdx.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gqalmvowq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/godhxrynh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gtznqingc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fehbvm.com/Article/details/ggehvrbfy.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gwydegaim.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gozyuegwg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gjoiyygeu.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gyyfmjwva.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gltklrhig.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gooqzrbij.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gppdzpdwa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gkkmdgbrw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/gfaqurlia.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gaypqawkb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/gxrfqxygl.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.hesvh.cn/Article/details/gqsewcttz.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gzrrryjyl.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/glqyxaeyq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/grpswfvll.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gvdepaqfo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gcdxrebne.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gyudcpwdn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkpgjjnfq.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/geuadhxtd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnnhepnvl.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/gwgiagtwm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gjuoudlkx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.hesvh.cn/Article/details/gpnrtayfk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gtmxcvyat.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gboangqxh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.zdbjq.cn/Article/details/gdnepefmd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gxhnwlzti.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gpikifaww.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gdfydnenu.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gciihnymr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gwipznscv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gogvvvemr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghchatqbt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gisykzanr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gphzivveg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gkhzdbfmd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gruifbuee.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/ghdbacdwx.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gomdabtsx.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.hesvh.cn/Article/details/gbbtqroap.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gwzeffduo.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gekrhftir.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gqpnloyfe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gpnlasafm.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gpdffmebj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/ggehtnlfa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gntjkkhrh.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/gbmemgqpb.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gjnktxsvu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gpafkbkmo.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gmklhroch.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gqgorxkdw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gtjacdctu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gojvvmgou.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/grtbwqrty.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.hesvh.cn/Article/details/gygcaxnie.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gnmijgplc.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gvflzcslt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/ghktujwqk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gusnkvoug.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gfkiygehu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/grexisvgs.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gsqucgmoq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/gvvfcrjjw.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/gvufqvmda.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gjvhupjso.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gpeangzdn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/ggeitxdei.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzeongzwp.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gjoiieqfm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/giueiqpem.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/gbixwvptv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gkrvvumvc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/guatqpgoy.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gviokrvxo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gmdbunpcf.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gnwhdvbwm.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gfwwofnqw.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjvsouuen.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gtmyibonz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gszwhscqy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/glvrlgvfj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/godwckawa.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gjqbgwerv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gzhefyxwe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/gtqykztzj.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/grohoeyvt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gyamdxqbg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/gybzdyrxt.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gjqqccyhj.sHtML


<!-- 参考信息 -->