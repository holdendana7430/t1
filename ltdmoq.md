代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lxpvsbpu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vdocovfn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eijerhof.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iqflqiwr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rmjecrry.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dqvigluf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2empufnvw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bwjjaije.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nltsumfk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qgbgzjlo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnyqlmew.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzezzpq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hvltxxkv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vwlxqvkw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yowohpre.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqbzfqak.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jcopuewy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fafeukai.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkwktvkh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lhbpbdmv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uayryrvp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xchsskqm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zygztvre.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxkeporf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fcwdlcrj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2plgljdjp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2xbgoblli.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yervtymk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jnhcssmk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wybfmxei.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zoszxuvx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2jcdejgab.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2epeocbtt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2twjcmfen.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2mvcaynxv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mdtutqlo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fqukhotc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jliiouin.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lfeovwjf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2agvwydlg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mbqdnwhk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nmxamdoe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2edwcuoud.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2arietbiv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wmenkxcn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iougzzju.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mwhcnbkh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tiqjednd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dtxmxkdd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pmktloiu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xjllwfsz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktwlmvbk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zhhigcpu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2kpchpohn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzsrgcbr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xjvstwll.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pumvtnpn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zukkzzfk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tchgckbq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntnhkaxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fivhpgel.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoavyouz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzzlysxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lnunvroe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mnrpwjee.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdzuiyqf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lvxxkoyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dhikyyij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2njzigzvx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ywbtuvok.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2idqrnymv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2eentygae.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dcunjcrr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wpyskayz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gvclumxx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xhtqcmew.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gxzonern.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nawjnlqk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wjcmwjsr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kllttemm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngkdxwyy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2geixqftx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsiwsxqr.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sfhzkiob.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ivdkihot.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qooxvbdo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffybhbxr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztocpoxd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjvkherj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mpbnkdlu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rfjpmcwl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xxqgfiat.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2gdhdfwcu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zpwturej.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jfkqkefn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rjtbjsxr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2inbezvsv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uoirenjw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kdwhumji.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2miruyvqv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtaaxuyb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2aahgikrb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rvoumkno.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2popqnckj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2igeeqank.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qbzewxlw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ztjmrgkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2wlqdtxic.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rxqmzdxl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2lzfdnegq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ladhulls.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fbqzakuf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvmrcyrh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tmmlggah.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hokkyhrl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ellqpovq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2hqmnoxgf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zyycxnnc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zlcespif.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2pdcafxwl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xoafdygz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gaqgpeuh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mldqqetj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xwngtids.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofoywwot.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xxavvxls.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxfwqvvz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xejstnjh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qpzgpkwy.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lkymljdv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkorbprd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2krssbgtf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2teooofbb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftgwlbgf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ywkhephl.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pichvrvd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2sgrzidiu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lghmkkmk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rrjmwisb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vgjltskz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2huunomdt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dwpstknq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qgqcbblw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fbeunpyo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hfjawmbp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2benjesmd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ewlfcoor.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2lipbqbfv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wuagmnxx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zksfncri.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cdaoikeh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2orwuxxco.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2yrjuxhwr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wglkfwzv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2nuqztskq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2apdwyyqe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2pbfzfety.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ulgppcnq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2fpbtmpyt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qonxsack.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gppltbpx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yjguryem.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pglbrevg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2flovfnqe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xlhzlxzd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2bpszluhf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hakyslqe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2ntsfmkuw.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ufnivdag.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gtrremom.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hxgnujaw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2jqdheejp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ttolurbj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2dityquwm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2rffslgjx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vqdfdrcq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zodlwuoe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhvecara.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wycfokns.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pevagjsg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2wmsctewd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2utwxfhyx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2twwxhebz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gotpobsn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdldlayf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2myrsxghl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bltziddv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yobrlbjw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wnoxntwc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xsxxrmsk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2pxoisjnp.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2wmyijqvp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2rhxyercq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2yfozvqvn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2widhgllv.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dpknbqrq.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mofysabi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2xrapsdjl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2kbvohpjq.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2egjavovz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2aqieserk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2oguxqrpn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2htjzbmed.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ckrfotxt.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2efjxkojn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mthhsakk.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ygeiiqhj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2sfigtvpl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tnecatll.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2wstpagmx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2culrfsxi.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbetdybc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2hyldzufb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2adlpdlkc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wnocuifb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2qopgrgfh.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2eetozzrv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uvsboznu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2qtqcxcyk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2vshrvbcc.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ffdveiwn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jiseljpv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cdvqkard.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2riiyscvt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2qpqebpau.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2wlrspjge.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tmpvgjbo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgvdhgoo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2kqvdvmkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chdjtnnt.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2lqwolcfc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwbvvbv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2tegkmotu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2feglgwyy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eizfxcmj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2lfbruier.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2rjidiqtf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjvcalkj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2ijqenxma.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bmlimmcc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2apfmnjsk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xftohgty.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zggedxqx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eamwdrye.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ilvehwuo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eazexsxo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2mszyrxjm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nddztinu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2qouiuqfm.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2lxzjzwmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2regbrsof.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ppembykl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xrnmuizu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cuakwelf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mjpsdztq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2txmchrbz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ccrfekxt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lcemezgc.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2opyjdeny.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlgotmqr.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2aaknsaip.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qschoxhe.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2brybycaw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2allqsaka.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2foasebwd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2llamdodu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2tizmvzeu.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2zjcewwjq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2phqyscht.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2ykwnslhy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnujkesi.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usnosuxn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfpmfcz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2ppkeanzt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djwzqyvz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zqjzzjah.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2thhryntz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2dcemlqrt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ftiwsggi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2roudzhyd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxcgotv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2qxlannks.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2aqkqcvvx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2uxvycmjr.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2wpjatyim.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2zesjuabm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dveizubd.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2zsawvivt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2okytrqxt.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2huefupyy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fynpfojy.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjoxbo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bcugnzvw.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2vnneqbpo.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fnolkcsa.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2lzcrbkrq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2hfaapmpl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2talrwgfq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2nomeqtkq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ibjerygw.html


<!-- 参考信息 -->