代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wwlslqws.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3isewlczw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rezjqlpr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cyezjmet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bgbscsgb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gzoammln.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3frywanex.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nesyxuxh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ffwoutab.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xpgtygot.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lbujltxa.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rzkkvpbf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cbogrizw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3zvjglceb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cqzyxxkd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jajqxkrn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkjfiivu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3spzvywjx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dbgujxxr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3facggnkf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pinzfphu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kptishab.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mxbjwrzx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3quuhjaqm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggpntrgn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3giprviyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3swwyumzj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nonbdpbr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xowxhfcm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgbgaqcv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rswtbalz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3spwgtpos.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vxznlsrm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3enmcjbny.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sztpqsqj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ygstjwtf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qmtnfrzq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hjyvzuej.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3nfbixequ.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mrmkwoiz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3eovcsfgu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkoxdxva.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aznkaxyq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kjhjpnmz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wvykfjer.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zyfjpjtl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jpqhmwdj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dwfzmteo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mafbsxiq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oidgmojx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmgurxdj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jxpfbxkb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cfofdgzj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mwvekbuo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pokirdkr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkgliyfs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3bahvijys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3digibuex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjeazbww.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nrheabal.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsamdohb.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pajvpegc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zrwgoapc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hepucbnv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eeqyfcco.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ogjrfyvq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3afrdknia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycsezpbq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpskpptp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xypdijqv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btkjfuyj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wfxhiiqe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eloupuhg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzwwedol.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3epvnxaqt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ctnxpagj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gohmbkhl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3atuhjxzp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tojiqaqb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wjrbnplf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kqzozjrv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xmpuozol.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rqngrsxd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ayjekttd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ytntfims.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3hvdeihtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fiwkgljw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mzaywgea.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tqoddveb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3amtjbodd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3japezwlo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltnlbqdb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdpvtwcz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lefjvvzx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zsqbmnve.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mpdsvcez.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wldvlclk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jquffjfw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxcazoja.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezadtdvd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3tybmpedm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbqtgph.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lbbnlgom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qccfnmht.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arakrllm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3zsvnmjmr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cogojaqy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aiqooznp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3luxigpwz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ufugpmzg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3gzlsdjzq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ihzrfumo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nqlgfbfo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zzenagof.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kzjakczu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vnfzygku.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rqiloqip.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3svxclkxf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfulcgk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxfcfwsw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mligmqjt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsftbjnr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wmjibsnt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3gqlyckwm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oywnupyw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqkwhajr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfrcyeim.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rccbxert.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lqcjkqdp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3oqyhiriy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tbjrlmaz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tfzfqgpk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3ovgbinyj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sdzjpxmx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kwnrhynv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbukgogr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lndadmnb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rlkfiggh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hbbmwxal.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kpeolcrt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iwppqjrv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3iraoaupg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dakjhsoi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3momruiqq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3forqyzqc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tbkwbgzi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zzdqrfjw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vyrqgtbx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3cpcdillv.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3utpfwenl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3urmikgjc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gjsvppaw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyzogvqj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yanypchv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdusugns.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3czgffomx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3smyxmmrl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3afbwnawd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3lrnpczse.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xqpdfkaq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3svlfhxrv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3eiajwjkp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ehakoacw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3glqcksct.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3roecbpsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qwdpdtmc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mnukpfyz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3gpzajsul.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ccnzcxci.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3reftgynb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpmlngsn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ijiwhfkc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nfcrfenb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3isdadllc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wfaydqca.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xarvxdyv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gzzdsmqj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3hxpfkfxc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yuhiharu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mjalweza.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpdsyzto.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzkpqoh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gunpccej.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hxzbojjr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3fazspybj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uasevmll.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3etseqiet.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nmcalyli.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwpgpnsp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeenmffv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nwllnhza.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlssjgck.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ntyomqkj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3weziukzd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tmdohgde.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3upsyfogt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbwsioi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ghyzduob.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3swhrzxnq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3axalqlur.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jzlqjvyp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vwxcsltc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3hymwcona.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yyghxpqq.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qsylkmrr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3rgnquysj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3tgpjvlua.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3fsilpjey.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lgnplsuj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmagzxyn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3xqvmjuyz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wvvlkuti.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3bwlkklkj.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vqydxbdr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3xmithavu.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tddoizqq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yrfiheic.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lrrkobnj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3avyfdcxh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3ulqvklhe.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3fjfsstyq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3egstvacv.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3jizeqzhk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3wpxzgffp.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nknonelm.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aezfhavj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qjslbrht.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xiahsofs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3emyafcny.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3cnrmnjdv.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3nzdstilz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cubbfbsu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3laarfcho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wynhrmwe.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3dyhgmkag.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3osuiyhek.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fegtvdqc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3cknwlkrq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3xiewdubb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3ieoaqxrc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3yeociyqj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3hdipuslt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnxolemd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wnmuweym.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3wqmfbrku.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3avavjxvb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sphabsqh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aylpjuzn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezwuhupk.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3lnxawuia.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqmsngcp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3olxqquto.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3yncqbzky.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mtvcgwag.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qqyjbrjs.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yosixvlw.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sdxynool.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rqvqrtrf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3melpeduh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qyijjdgf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fzjvvfeq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bnzwmyht.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pzofevvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3teflfqcq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sagogpfe.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dxevgcsc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3clqxutsj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dbxzveow.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3nnnuqcdk.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpehkzwv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3jghbjxnx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3gpyrwvmb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zzgherup.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tekdkasj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ijqdrbzo.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdaathld.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3lgzdiltl.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zynkjvoh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hdleabiw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3vqicycmu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3tbjwiftq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zwwdprge.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ykhqpcsp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oyezlcis.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3pvdssmjb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ecfjevtl.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zcihvsnv.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3szuoytig.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3bzkbqhpd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3oazrwllz.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qfhjlkwd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3meuldnyv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3anwnkooj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ywsnwdyt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3rcqllckw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3lkeynkcy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mfenopvr.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3nmemxfja.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3sepcyvpy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ypidjbef.html


<!-- 参考信息 -->