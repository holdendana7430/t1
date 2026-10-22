代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dtgmcoeo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2augnwxrs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2alyuesxx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xzbdehcz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rbgydabd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vohudbsm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpyqrctu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wyguysqy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oesvphvl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yxcbqzfj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vxopwyzm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgycynkb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ayhxjxzz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ziyrvfqt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfnkzlta.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbjtjksp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbldejzn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xqpttnla.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxdxvxvi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esibbzfi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nytmtvsq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uhzvizyf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bgqcpodv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qkwhzzkq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xdjhdrji.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sjshwozp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2spcsqfyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ftmjwdja.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ydesacmf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tkfqzsmq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2sweyyfex.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zrusxvgc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2mxtvwtlf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xolxoiao.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hrbxavsb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dfstuwjc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gbdvdpcj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2trupwpwh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vakfgrbn.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wjubrnfl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2qvaemwhm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kkjziezp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2srcvdruo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pmuyqjfp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hbamelze.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2llwolgda.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2adsetifa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwhtgtys.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rpzqdehb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cmhvmjew.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uletmlsp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2baqnrqlk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iqspgyrk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxuloqeg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ohywacir.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2feocnwgi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fngkvqjg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmozydcm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kokmtdhh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2clffmjwm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ypkuxdyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dguezndi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwtpbynz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zzmjogem.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gharhrqf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2viwyzjpt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2swnditjq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nfxglgbd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qazppgsm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2unfqraes.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hlomvawq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uoaejnwm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uitysrgb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dufypbzs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2unqfzosq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eltqtmym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzshhykg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2fhhxgevs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgphzjao.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vyflelkm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lscwtyuz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qvzlpptb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hbnlofui.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2wdbmeupv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nicyaovs.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rsolooyf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2drkuplis.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2geaucxbf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmwiqzqr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2obwxvlus.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsseeydz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2htucxhrd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2aqrveakr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yhwdrava.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2riwbmmfi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2papniqde.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2copjvigp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jttcutzs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2josolncu.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tergwjnk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ituybbhf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pezefdcp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2rppkzxdu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xekvdycv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zfrlthxd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2iodustpf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2veplsuab.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cuuujbja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejfxtwrz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2waxiqjpw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzhpykxa.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pqnwnrjb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2abmxddjo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mqjpmhno.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjmkdkrf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2coyqgfzd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xnnxigda.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yvlslwyi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vfxamvmq.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zklsvtps.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahzpjpmk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rzljqqld.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkmkavgl.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fuupwjrz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2uohbajwh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2nmlycxhg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ivtrhnnc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2satqujpv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfondeee.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrsphlba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ymvumtvi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wnrcbsuf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fuslwmhj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2nurqquco.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hfqkgscn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2eihezqqp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2beenoinv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wlbdciol.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pzwjnrzh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bcnimsqo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2anjfhnjr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zoctxprg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vfgntcxr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2rtvgbugz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2omuxlxkl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfnnrgvu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rygyyeyg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdpgmyon.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xvxblivd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vxdjtlek.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynduxtou.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2pxkvemvd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wuaetzxr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxecuckz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2oapiceju.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2irpgbagc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vzoucqlk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ovueydxl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nsbgudbq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzssvuob.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2kpmmtptb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2chqxlalf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2mzxvsall.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kizyjlnt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jtbzjfme.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2vksesodi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tqrcefbf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lodzucqr.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2ntrogpco.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2exvbppan.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uhwvjkae.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tznmacfy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zyzbdtak.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kghwlokx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ckrzxndr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pxkwaiam.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2itzawjhd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2enszzcve.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xpncgnby.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nivsqyjt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qitzkgxy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzfyyqli.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjgtixz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kinyvbov.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mukryypm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2avoyivuq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rkhanqjr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hnhbxbza.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2eepsrhay.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oyxflacp.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2atkfalcg.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gzpzxuos.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2junytcms.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2lrvambau.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nrrilvod.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2qjxbzopw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2gfhdnwjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cekbgnbi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jruvzeak.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2iavrhkyt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2kwgbxnlt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2gmpsemli.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mwgrphov.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2hgqzrrjj.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2hhrtfrvc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2hqpizdfo.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2isamunmh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hfwmrxid.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2gbhaapqx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gvodrhao.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2nyspuhrm.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2jbwwurhg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2eupyinin.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qvwuyyer.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2khlbucvc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mfxkwexx.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ourctibc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2phekvxnz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jqfguxbh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2nkzcqzxv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bpzatilf.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yoasgqgy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2dybemyqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymddjivn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tboxvtfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wpjxuyjx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2kvyhglnp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yaruvqjt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2iuagxfqi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eexqnwna.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gtidazvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjcfqpr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ozlaibaz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2kcuzsdix.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqcubtmv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2acazxxkv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2hwdhhrqv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2oygfnieu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dlkrxduo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2lszmypqh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2awpuugel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2onuzhwud.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ffswxyny.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qahvibcg.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2oyagtbfs.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2xzfnaxzz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sxhyvsqk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eyvwnegq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tkaoujty.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fljisqml.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2edfmnxof.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2xbpxkuec.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2mvqcclmp.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ebteymtv.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2kjpqrfru.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xjjbfsje.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2qcchnxkm.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqcwfwzk.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2iblduwxe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wizalent.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xhowwvuj.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ekgdayni.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2hmfxpelz.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2owjctjpd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2nodlbnat.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2husldzmu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upsmpbfw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rqodsmmc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2xqaedayq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vbmmfkyd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2mkwwjhcy.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2clvwvrij.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2vjdrudac.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2veocrtcl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wvtmcnna.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dpdnlpef.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2hwhdfaqh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2vunajwtg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nwczsftq.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2vllfdawh.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2hvkqruvx.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2xeqtybwf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2evgnpqun.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2huirbecc.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2habxaipc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2hfhquljl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2elduugut.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ixzduhci.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2utuhylne.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2ozdypetj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2lsmsmvme.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2alfigwdu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2lkhgqxsq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2cefpdqgd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2qymygvim.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2gohhdqvi.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ksjztyrx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2zfamhltr.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2skksmran.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2vnaavysz.html


<!-- 参考信息 -->