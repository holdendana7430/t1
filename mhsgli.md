代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2cpxnxaws.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ovoasniq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ttpxtvba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qrzbeikk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rkdssytc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2duqwjfdi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rgneenrq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrkdjhlk.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blpljicv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jesqziwz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2wtoczjpw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjvtocju.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkiujygs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ixxqtody.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2izuhftdl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uzzwssiy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kslryzur.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfvnenxj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rnmmtluj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhcyzaqn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvxgskss.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aqkeroua.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mvipxazh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lxbduhpm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2etsqybgu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mljsyekk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kcfidauo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rufnmvii.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2awbbzlbw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvbryky.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2noiyqziq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2miioukox.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oxjbcbcj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2wecjzzus.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2atuvzdai.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nzvetqxt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hgpkuqeq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hgssozhu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hmramgqe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnsltnd.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2biofvqyh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsexkjak.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rnmoyehf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2efyzvecb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hskbwxoo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2isrgxiao.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2zvdpuzgx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpklanec.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qdncduwu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2shfvocmu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzqkphox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2acgvsubd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jgxqmpdx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqjquigu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wvewuoqg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akfoshrz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndnvgkkq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgccysjk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlxbsjjj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ojcpbyeo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mwbabvkx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qogolycw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2enxmqfgo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mjcorbnr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yxxcuqlc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rftepoug.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2srvxhohe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2oqcxmczp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lvsjklni.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zqtruyud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2frssliuo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gdnxkfkb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2cpnlifke.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ehiqjsbo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2udqzkhio.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2eohzwajr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2smdjifxm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gvmcgzux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctbbavzo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fiaxucwj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hngwyzdz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzdcwqkc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jfbhfysz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqcirfgi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2chkjbhul.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pvafjngx.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2amlitejs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2isszblkm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eaoxmtpr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vwvpvrok.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsailcji.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnvyxqci.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2cdujcqgo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymsslmat.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kwyteyps.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ervkmngf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2njsularh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qojcjtqn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ixsowcaa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2exykphrf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xqppltzp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2phjderjf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yujavafn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2rwiwogfj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2llmtegvn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2wrvkvqsq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yvbfvgzl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gfittxtn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kzkokxtv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tkgnxcro.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ztyyunar.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2shyvsfwe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dcbdvxsg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2unzibmpx.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nkuidghw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2flvjccfa.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wnovmmfb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mihetrxx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2paaelnpa.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vezpcbfo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2taiwalag.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lxkzzlac.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dggmxbut.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cduzkclu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2szkivyaq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tzdhggtj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzwleqfn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ewjgnzjf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qsvvdraf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kmywfhfb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ybjjvzlx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjvjrwwr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ikyfasxl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ugrefdia.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cyhzulip.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lqfhdvjr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ogiylxbv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fyrankml.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yddrsjym.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2iqpufpvu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2iaesijep.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2axcqvogk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lmhbpmzm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jrtmogiq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nminvsql.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2chpcjbit.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayvvulda.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2juozlupr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mlnvoxuu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xzlgdupp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiluasya.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yvhdfgbx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2uhpnjswi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2ofwalduj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qiyrrjbc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iykrdbgx.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vowdecwd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hxrlijhy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2edqncdyb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dutamkks.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2roynpdik.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2glhwqhbq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gxzommtb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bysiepqo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ipmjctqp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2rmhykkup.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gaanbbzf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rzxrmils.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rllklbgi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qmtobofs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xpmqiqpw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqnjoetk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2taniyfah.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2qtplybgs.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auwjbryv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2avdryzzd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aycdqtda.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ismwfmlp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fhsjkamk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2amlvmwfm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbhpvr.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hgqjuzbc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxcjyxob.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcchgmzw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jwcnzcst.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nerggosq.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ogmcmzio.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2aevcaclt.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2annzijtw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pnkjxrnr.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dapdvdup.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tsilajyp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2flwtjrro.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dzppmqip.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2huzauwtz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2baiblzie.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2pghgpepr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2hzapbcrh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ongnzlth.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2htznuuri.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ontrkgaf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcszaeuw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2qsozmgvs.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2myuvlknf.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2mirjfvaz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jcihrqts.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lqgparsc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lucrffmb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lxzgvprp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2gqlkhoig.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2wbojwwdv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2vamreweh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2whsjvmax.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmeknefe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2avdjuxlx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2khpnmxay.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2wfpsqede.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ssrsqsyt.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uaozhyiv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2auhgylij.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2oyjsnogl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ztjombin.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nhztqwar.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hujzcvno.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2hyjeaipv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsvrxeog.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2tgtiyvzb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2bvbozwhl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bezymchz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwyiwdkl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmfxlufp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zhxlpgyp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2cndoryqe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjvuzuue.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2vyqucbkb.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2utoreppz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xmzkgkfe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2frrpxkpa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pfutfpek.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otkemjud.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynghdfnf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ptaujvhm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qutwsykl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jobdzuqy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fwarsodj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2iskuypqm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bxpfmdvn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zgdhfycn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2keokjjix.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2oinnnpby.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gafdnfof.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fjboggzy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2zkagwfva.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2phrarowk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tvprvzvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2emiazebk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtccikgr.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2frhiuynt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2bgoilavb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2egobmyda.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2qyjtxzay.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uuochhpf.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2dbizhekq.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fpdcrksz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2hzkrmhqx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bezjphof.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2wgvrzhlh.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wakznovu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ukcdtvnx.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2ttztkqgi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2yyfkiwud.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2uinoqcpu.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2tzixqgpz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ifnzoskx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2sgwnacra.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cntbjuqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jvxncfsx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwncikk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2pfnrsdlc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2qkhskhmd.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2qabqbvjp.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2udiehvpp.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iobszvgs.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nmcdomwt.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gbqrgoin.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2gfgjrfbj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2saxlduey.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2krlcjthf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tszpmgvt.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2futpwlcw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2pjgzxzhw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2cnftekjf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kyyacuhd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2irypltnb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2vzrjpygf.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2bkuhmorc.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2btrgbybw.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2pqlxkvdt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2twktugjh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2gwinqugk.html


<!-- 参考信息 -->