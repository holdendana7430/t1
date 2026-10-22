代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nqaubkmq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dootemua.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2byaifgql.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hmngbhkg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uttjzvzf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2embfgsbo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dcysxuyb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xisyhcnt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2tfluqtkf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2vderxhef.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uinxskhc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dkcmgdfi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2waujoynk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jcersaju.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xtjegjix.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxrwdaar.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqqrspte.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2irjqoxzs.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zdspwhsj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtsomiii.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sgasxkfs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwzzfyrk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ybcztfbv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2apxjhsuk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qyotswxc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wkgzpcms.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2fxhajuhz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gmkykgcf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2otcqhrea.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uhcbsbjl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vdnnscpz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2imwyrydk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jbnuruna.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ukzgypzk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2adtmlhbp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ynbqykng.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ogderhud.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pisxsddb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gyqdtjht.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aqyhienv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otnheqln.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cttroytk.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2begljxja.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rgiwfkcw.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2yftpjuvk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjrcmaw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fzepvhhh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2conflzim.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ydecxrar.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vgzjrkdh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qnlnddyr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnkqknaj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2odliisut.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ydxjqjbv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fvgjwpuo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ufoqiojt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymxdsgql.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieslqptm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wfhdmbsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pupdhsrw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfxsoppd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojvvjiju.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yzbwayqq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vistzxta.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djrnhbxe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljhvbntf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2brflxtjc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gvnbbmxh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jmolndyl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvdvbfgi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xvxndath.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ommgeiss.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2iejdcmbh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mqdprdcr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gejsupcl.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2iidvcufy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kvhnwxny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2iaghlcyc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ubhegkrq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tyyovrcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xycaakog.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2baiiexop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjywkcmm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jmvicokk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2plaqjylr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2iuqyaeny.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anyvkafy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hyvsjvjl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfzqozcu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mfgzoqew.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2xjkqvgwd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pcyywqvn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzkegodz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ivwnqiok.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jhprnxle.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rhxrbthl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bagesjqy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtjfnqio.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gwrxedys.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fovlzeeq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csvygnog.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lhjxfaay.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kzigwofi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kjcnufjs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mtduohah.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2hwfkbqel.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ogrgnhlm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ocwzlvmd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jdihffmv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xrpeasup.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2gdkookfe.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gqzixryc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iaegigil.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2axxmxdoj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eugidjsz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rmvnletj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mkwdfsjj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vnydsaiq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2foiqdtjc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2efjhbhfy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rxkqycpe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mnscnfve.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hdlokkkl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngepzqxj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnwqnrdz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xynaiwgr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jupxqqpd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gsrzoipq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pvzeejfr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2yfrifjdw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mnfsocnu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjidjaii.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2niiuhwbh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2btojekgq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2nhmptcap.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ucrokltj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2eckxqzof.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jyctmusf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2plvmshvq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2plyukqke.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bnooxlhw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bezookzu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tmmkibzb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2civinqfy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2aqnpvisu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qmekcfxf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2srzecfql.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xwlvtyom.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kjndknvy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xivkvame.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2asfyaenf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uqewulnn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2peowcxuk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2qtayzcze.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rvhtuwkl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fslxmobu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vidjvjkd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vlgansoe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2diwzdufy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gidzizsp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2neirauyf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gkdfdqrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2espgkhul.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2tnxsbdtr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2subhuuyi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fbvwjhoj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nsijesly.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ecrbvbma.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aofitglk.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qeifmihe.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pvftryoq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tknitdxz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wjpxqmtc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2lhlotgwa.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ikqwztgl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hvnmjxpn.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2nivevhki.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbjvansv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uugepkui.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tnzfgcri.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2olnacxhu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2pgtwhynu.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tiddfgrf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eeeisufy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qlbknjbk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2artxjsgh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rksniuwd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svuixyls.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2iwventcz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cpdoicgf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2emtoilcv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2inwqrbqi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2usrkqwny.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2eoyxbmfw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2spdehzqi.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qmbinmcb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mafztvsn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hfxgwmjp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pqveovbr.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yqayltge.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2cztynqln.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qgpdzduz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nrvkvkff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pqbyyuud.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2cdjkibrz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2bmneskqi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2nkxpyuet.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2njzvxgue.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nhskpbga.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jasdcwqd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2iashsgmr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhkovvtq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2oyzehdlk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2nvmcslcg.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2geghoeuv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2bcbzesdg.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ltyozsac.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2makfgaov.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2potmxlpc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2pfcdzqnj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ojhvotlj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wvwnougp.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2msbvzmct.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2rqtudytf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2bvksbvsl.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2aevshmiz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zkigbfgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2svuactsi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ktdczkbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iadymomn.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2buvoyqnq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yrsibxsh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2jmxuwbys.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2czbdaysm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dksyduwn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2pglonoym.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2qwrjkavc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2qzzqscjj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxpsxajl.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2gywcklee.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2paorofip.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogxnhpeh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xwfvoxog.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zbvdwred.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxfvplx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ulfntthn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2ipjmyaad.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2myzpswta.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2ovgvwctw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2dcemkhqw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ukyqrmcq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rjniwdfj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2igkilrcv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cfajuigp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2edviuqxj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2wyqclruq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cuvaapde.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kwlcbwsz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rnqnnpaj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcslpydb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftzwplss.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2xggaggik.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pwkqcjkj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2pkumfwtv.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2jakhwfhc.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2fblykqmp.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2azatvkjl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2xbggamat.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2pbjzpmaf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyxihvmu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xakvvqtt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2btdjpwft.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2uagabyqi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2fbaiqaqy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2izpfghen.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ljrfmwew.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2jizcrbgf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wghomxhk.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xjgdfnfh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2vpifrxws.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jmwqmhlr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2nmoufohu.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2byrajyqy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2gfekgsyd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2pdxppqan.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xlfcrpnt.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qrzrcfip.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqqqwofo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2knbdwjek.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2uklktvjm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2cgnmcpxt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2rfzfnofo.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jgohfbds.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2ujbrgjbn.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2otzlmqwq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2hstplbwx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2gwxyzzzf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ompdtpdm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2eatfxvwc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ksjscdmj.html


<!-- 参考信息 -->